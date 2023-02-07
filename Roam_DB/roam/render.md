[[.--]]

## Articles::

### [A closer look at roam/render](https://www.zsolt.blog/2021/02/a-closer-look-at-roamrender.html) by [[Zsolt Viczian]]

{{iframe: https://www.zsolt.blog/2021/02/a-closer-look-at-roamrender.html}}

## Examples::

Code:

```clojure
(ns md.example
  (:require
   [reagent.core :as r]
   [roam.util :as u]))

(defn parsed-text []
  (u/parse "[[Pages]] ((uWcJicabj)) and [link](https://roamresearch.com)"))```

Rendered:

{{roam/render: ((FFwfsxVY1))}}



Content #.h

```clojure
(ns roam.keycommand
  (:require
   [clojure.string :as str]
   [clojure.core :refer [println]]
   [reagent.core :as r]
   [roam.util :as u]))

(defn includes? [s1 s2]
  (when (and (string? s1)
             (string? s2))
    (str/includes? (str/upper-case s1) (str/upper-case s2))))

(defn includes-strings? [s strings]
  (every? #(includes? s %) strings))

(def help-content
  [{:category  "The Basics"
    :id        0
    :type      :key-command
    :functions [{:name     "Find or create new page"
                 :shortcut {:mac "cmd+u"
                            :pc  "ctrl+u"}}
                {:name     "Bring up quick commands"
                 :shortcut {:mac "/"
                            :pc  "/"}}
                {:name     "Reference or create new page"
                 :shortcut {:mac "[["
                            :pc  "[["}}
                {:name     "Reference a block"
                 :shortcut {:mac "(("
                            :pc  "(("}}
                {:name     "New block"
                 :shortcut {:mac "return"
                            :pc  "enter"}}
                {:name     "Indent block"
                 :shortcut {:mac "tab"
                            :pc  "tab"}}
                {:name     "Unindent block"
                 :shortcut {:mac "shift+tab"
                            :pc  "shift+tab"}}]}
   {:category  "Formatting"
    :id        1
    :type      :markdown-key-command
    :functions [{:markdown "**Bold**"
                 :shortcut {:mac "cmd+b"
                            :pc  "ctrl+b"}}
                {:markdown "__Italics__"
                 :shortcut {:mac "cmd+i"
                            :pc  "ctrl+i"}}
                {:markdown "~~Strikethrough~~"
                 :shortcut {:mac "cmd+y"
                            :pc  "ctrl+y"}}
                {:markdown "^^Highlight^^"
                 :shortcut {:mac "cmd+h"
                            :pc  "ctrl+h"}}
                {:markdown "[Link](/#/app/help)"
                 :shortcut {:mac "cmd+k"
                            :pc  "ctrl+k"}}
                {:markdown "$$\\KaTeX$$"
                 :shortcut {:mac "$$"
                            :pc  "$$"}}
                {:markdown "# Heading 1"
                 :shortcut {:mac "cmd+opt+1"
                            :pc  "ctrl+alt+1"}}
                {:markdown "## Heading 2"
                 :shortcut {:mac "cmd+opt+2"
                            :pc  "ctrl+alt+2"}}
                {:markdown "### Heading 3"
                 :shortcut {:mac "cmd+opt+3"
                            :pc  "ctrl+alt+3"}}]}
   {:category  "Navigating"
    :id        2
    :type      :key-command
    :functions [{:name     "Move cursor to next block"
                 :shortcut {:mac "down"
                            :pc  "down"}}
                {:name     "Move cursor to previous block"
                 :shortcut {:mac "up"
                            :pc  "up"}}
                {:name     "Go to Daily Notes page"
                 :shortcut {:mac "ctrl+shift+d"
                            :pc  "alt+d"}}
                {:name     "Zoom in to current block"
                 :shortcut {:mac "cmd+."
                            :pc  "alt+right"}}
                {:name     "Zoom out to parent block"
                 :shortcut {:mac "cmd+,"
                            :pc  "alt+left"}}
                {:name     "Go to next day\n(when on daily page)"
                 :shortcut {:mac "ctrl+opt+n"
                            :pc  nil}}
                {:name     "Go to previous day\n(when on daily page)"
                 :shortcut {:mac "ctrl+opt+p"
                            :pc  nil}}
                {:name     "Go to first block on page\n(when nothing is selected)"
                 :shortcut {:mac "cmd+return"
                            :pc  "ctrl+enter"}}
                {:name     "Go to last block on page\n(when nothing is selected)"
                 :shortcut {:mac "cmd+shift+return"
                            :pc  "ctrl+shift+enter"}}
                {:name     "Follow link under cursor"
                 :shortcut {:mac "ctrl+o"
                            :pc  "ctrl+o"}}
                {:name     "Open link under cursor in sidebar"
                 :shortcut {:mac "ctrl+shift+o"
                            :pc  "ctrl+shift+o"}}
                {:name     "Move cursor forward"
                 :shortcut {:mac "ctrl+f"
                            :pc  nil}}
                {:name     "Move cursor backward"
                 :shortcut {:mac "ctrl+b"
                            :pc  nil}}
                {:name     "Jump to start of block"
                 :shortcut {:mac "ctrl+a"
                            :pc  "ctrl-home"}}
                {:name     "Jump to end of block"
                 :shortcut {:mac "ctrl+e"
                            :pc  "ctrl-end"}}]}
   {:category  "Blocks"
    :id        3
    :type      :key-command
    :functions [{:name     "Move block up"
                 :shortcut {:mac "cmd+shift+up"
                            :pc  "alt+shift+up"}}
                {:name     "Move block down"
                 :shortcut {:mac "cmd+shift+down"
                            :pc  "alt+shift+down"}}
                {:name     "New line within block"
                 :shortcut {:mac "shift+return"
                            :pc  "shift+enter"}}
                {:name     "Expand block"
                 :shortcut {:mac "cmd+down"
                            :pc  "ctrl+down"}}
                {:name     "Collapse block"
                 :shortcut {:mac "cmd+up"
                            :pc  "ctrl+up"}}
                {:name     "Select current block and children"
                 :shortcut {:mac "shift+up"
                            :pc  "shift+up"}}
                {:name     "Select block above\n(when block selected)"
                 :shortcut {:mac "shift+up"
                            :pc  "shift+up"}}
                {:name     "Select block below\n(when block selected)"
                 :shortcut {:mac "shift+down"
                            :pc  "shift+down"}}
                {:name     "Select all blocks on page"
                 :shortcut {:mac "cmd+shift+a"
                            :pc  "ctrl+shift+a"}}
                {:name     "Copy block reference(s)\nof selected block(s)"
                 :shortcut {:mac "cmd+shift+c"
                            :pc  "ctrl+shift+c"}}
                {:name     "Cycle TODO state of\n current / selected blocks"
                 :shortcut {:mac "cmd+return"
                            :pc  "ctrl+enter"}}
                {:name     "Open block search"
                 :shortcut {:mac "ctrl+shift+9"
                            :pc  "ctrl+shift+9"}}]}
   {:category  "Sidebar"
    :id        4
    :type      :key-command
    :functions [{:name     "Toggle left sidebar visibility"
                 :shortcut {:mac "cmd+\\"
                            :pc  "ctrl+\\"}}
                {:name     "Toggle right sidebar visibility"
                 :shortcut {:mac "cmd+/"
                            :pc  "ctrl+/"}}
                {:name     "Open page in right sidebar"
                 :shortcut {:mac "shift+click"
                            :pc  "shift+click"}}
                {:name     "Open mentions in right sidebar"
                 :shortcut {:mac "cmd+shift+click"
                            :pc  "ctrl+shift+click"}}
                {:name     "Create page in sidebar\n(from search)"
                 :shortcut {:mac "shift+return"
                            :pc  "shift+enter"}}
                {:name     "Open link in sidebar\n(when editing)"
                 :shortcut {:mac "ctrl+shift+o"
                            :pc  "ctrl+shift+o"}}]}
   {:category  "Appearance"
    :id        5
    :type      :key-command
    :functions [{:name     "Toggle display of\ndouble brackets"
                 :shortcut {:mac "ctrl+c+b"
                            :pc  "ctrl+c+b"}}
                {:name     "Toggle display of\nall inline mentions"
                 :shortcut {:mac "ctrl+c+r"
                            :pc  "ctrl+c+r"}}
                {:name     "Toggle all users' bullet colors"
                 :shortcut {:mac "ctrl+c+s"
                            :pc  "ctrl+c+s"}}
                {:name     "Toggle other users' bullet colors"
                 :shortcut {:mac "ctrl+c+c+s"
                            :pc  "ctrl+c+c+s"}}
                {:name     "Toggle block live preview"
                 :shortcut {:mac "ctrl+c+p"
                            :pc  "ctrl+c+p"}}
                {:name     "Cycle namespace display"
                 :shortcut {:mac "ctrl+c+l"
                            :pc  "ctrl+c+l"}}]}
   {:category  "Other"
    :id        6
    :type      :key-command
    :functions [{:name     "Toggle help popup visibility"
                 :shortcut {:mac "opt+shift+h"
                            :pc  "alt-shift+h"}}
                {:name     "Undo"
                 :shortcut {:mac "cmd+z"
                            :pc  "ctrl+z"}}
                {:name     "Redo"
                 :shortcut {:mac "cmd+shift+z"
                            :pc  "ctrl+shift+z"}}
                {:name     "Move character under cursor forward"
                 :shortcut {:mac "ctrl+t"
                            :pc  nil}}]}])
(def PC?
  (when-not (nil? js/navigator)
    (not (str/includes? js/navigator.userAgent "Mac OS X"))))

(defn key-command-view
  [{:keys [name shortcut]}]
  (when (or (not PC?)
            (and PC? (:pc shortcut)))
    [:div.rm-help-function
     [:div.rm-help-function__name
      name]
     [:span.rm-help-function__shortcut
      [:code
       (if PC?
         (:pc shortcut)
         (:mac shortcut))]]]))

(defn markdown-key-command-view
  [{:as   props
        :keys [markdown shortcut]}]
  (when (or (not PC?)
            (and PC? (:pc shortcut)))
    [:div.rm-help-markdown-function
     [:div.rm-help-markdown-function__style
      (cond
        (str/starts-with? markdown "###")
        [:span.rm-level3 (subs markdown 4)]
        (str/starts-with? markdown "##")
        [:span.rm-level2 (subs markdown 3)]
        (str/starts-with? markdown "#")
        [:span.rm-level1 (subs markdown 2)]
        :else
        (u/parse markdown))]
     [:span.rm-help-markdown-function__markdown
      markdown]
     [:span.rm-help-markdown-function__shortcut
      (when shortcut
        [:code
         (if PC?
           (:pc shortcut)
           (:mac shortcut))])]]))

(defn content [_]
    (let [*query (r/atom "")
          *selected-category-id (r/atom nil)]
      (fn [_]
        (let [split-query      (str/split @*query #"\s+")
              filtered-content (->> help-content
                                (map (fn [category]
                                       (assoc category
                                              :functions
                                              (filter
                                                (fn [{:as   function
                                                      :keys [name
                                                             markdown
                                                             title
                                                             description
                                                             shortcut]}]
                                                  (or
                                                    (includes-strings? name split-query)
                                                    (includes-strings? markdown split-query)
                                                    (includes-strings? (:pc shortcut) split-query)
                                                    (includes-strings? (:mac shortcut) split-query)))
                                                (:functions category)))))
                                (filter #(> (count (:functions %)) 0)))]
        [:div.rm-help
         [:div.rm-help-search.sticky
          [:div.rm-help-search__icon-container
           [:span.bp3-icon-large.bp3-icon-search]]
          [:input.rm-help-search__input
           {:placeholder "Search all key commands"
            :value       @*query
            :auto-focus  "autofocus"
            :on-change   #(reset! *query (.. % -target -value))}]]
         [:div.rm-help-results
          [:div.rm-help__left-panel.sticky
           [:div.rm-help-categories
            (doall
              (for [{:keys [category id]} filtered-content]
                ^{:key (str "category-" category)}
                [:div.rm-help-category-menu-item
                 {:class    (when (= id @*selected-category-id)
                              "rm-help-category-menu-item--selected")
                  :on-click #(let [function-group (.getElementById
                                                    js/document
                                                    (str "rm-help-" id))]
                               (.scrollIntoView function-group)
                               (reset! *selected-category-id id))}
                 category]))]]
          [:div.rm-help-functions
           (doall
             (for [{:keys [category functions id type]} filtered-content]
               ^{:key (str "title-" category)}
               [:div.rm-help-functions__category
                {:id (str "rm-help-" id)}
                [:div.rm-help-category__name
                 category]
                [:hr]
                (doall
                  (for [{:as   function
                         :keys [name
                                markdown]} functions]
                    ^{:key (str "function-" (or name markdown))}
                    (condp = type
    					:key-command          [key-command-view function]
 					    :markdown-key-command [markdown-key-command-view function])))]))]]]))))```

