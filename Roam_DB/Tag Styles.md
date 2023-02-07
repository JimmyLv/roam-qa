Links and tags whose name begins with a `.` add a css class to the roam block that they are on

This can be useful for [[Use Cases]]  like

visually organizing your day if you track your time

Try it out

{{[[roam/css]]}}

```css
.morning-routine {
 background-image: 
    linear-gradient(
      hsla(4,90%,58%,0.42),
      hsl(45,100%,51%, 0.6)
    ); 
}

.break {
   background-color: #607D8B59;
}

.increased-emotional-energy {
  border-right: 4px solid green;
}

.decreased-emotional-energy {
    border-right: 4px solid red;
}

.ramp-up {
  border-right: 4px solid;
  border-image: 
    linear-gradient(
      to top, 
      green, 
      rgba(0, 0, 0, 0)
    ) 1 100%;
}
```

[[Example]] Top Level of your Daily Note 

Log

06:00 - 7:00 #[[.morning-routine]]

7:00 - 8:00 Great writing #[[.increased-emotional-energy]]

8:00 - 8:30 Frustrating Meeting #[[.decreased-emotional-energy]]

8:30 - 9:30 #[[.break]]

9:30 - 10:00 Getting back in zone #.ramp-up 

What you'll see if you hit turn on the [[roam/css]] [here](((Wk2cMCJjJ)))  ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2Fkb6T9fa4hH.png?alt=media&token=5fa2ddf7-7370-4868-b31b-2961e51b147c)

Taken to the max, they can pretty dramatically change the layout of particular your blocks in your graph

{{[[embed-path]]: ((Nt3syyeHc))}}

Roam ships with these CSS libraries built in, so you can play with classes from them right away

[[TailwindCSS]]

Blue background, white text with `#.bg-blue-500 #.text-white` #.bg-blue-500 #.text-white 

#.text-xl larger text with `#.text-xl`

[[Blueprint]] 

Card is probably the most useful by itself `#.bp3-card` #.bp3-card



