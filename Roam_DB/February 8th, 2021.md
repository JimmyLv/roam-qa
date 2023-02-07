

[[Hiring]] [[Work at Roam]] [[Clojure Engineer]] - [[Backend Role]] [[Take Home Project]]

{{[[TODO]]}} Given a map, or a [datascript](https://github.com/tonsky/datascript) database at two points in time

{{[[TODO]]}} Generate a diff of the two structures

{{[[TODO]]}} Generate the minimal transaction which will bring A -> B, and vice versa.

#Bonus 

{{[[TODO]]}} Given a set of User-Events which map to certain transactions - find the sequence of user events which brought A -> B, or which would bring B -> A

{{[[TODO]]}} Take a roam outline tree, and create a datascript DB with just the data contained within it  - such as this one This item

{{[[TODO]]}} Publish your code and the demo on a roam graph using `roam/render` and custom components

Roam allows you to write arbitrary CLJS code - and evaluate it in your graph - you can use this code - and the roam Alpha API to query your graph, and create mutations for it.

Submit your answer as a roam-graph

All code should be in the same Roam Graph as the working demo.

{{[[roam/render]]: ((uP_2barEP)) ((cpgzSMTye))}}

```clojure
(ns starting-point-for-custom-roam
  (:require
   [reagent.core :as r]
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))

(defn x [{b :block-uid} x]
  	[:div.bp3-card 
     [:ul
     [:li (pr-str @(dr/pull '[:block/string {:block/children ...}
                              :block/uid 
                              ] x))]
      [:li [:h3"Schema" ]
       (pr-str @(dr/q 
                     '[:find [?a ...]
                       :where [_ ?a _]]))]
     [:li (pr-str (keys @(dr/pull '[*] [:block/uid b])))]]]
  )```

This item

Has children

A

B

C

## IF you want to also be considered for  #[[UI Engineer]]

{{[[TODO]]}}  generate a UI for displaying the diff 

{{[[TODO]]}} create a simple component that will let you save the state of a block subtree at various points, and return to these states - by firing new transactions

Import

[[December 1st, 2020]]

From: December 1st, 2020.json

