---

title: Vertices and Edges (An introduction to graph theory)
permalink: /2017/07/10/graph-theory-introduction
author: Jeremy
date: 2017-07-10 04:19:09-0400
---


An interesting area of mathematics is graph theory, and it deals with a simple question: how do things connect together? In graph theory, we're interested in vertices (also called nodes) that have relationships with other nodes. These relationships are called edges (or branches), and with these two ideas, we can explore many different and interesting problems. However, the reason I'm bringing this up now is that I've been watching a superb series of videos that explain the workings of graph theory, and I wanted to both share the series and comment on some of the problems. To do this, we'll have to go through a bit of the theory to ground ourselves comfortably, though we won't go into enormous depth.

But first, the series is called [Bits of Graph Theory](https://www.youtube.com/playlist?list=PLGxuz-nmYlQOiIOriTXMEoGoybUC3Jmrn), and it's created by Dr. Sarada Herke. I'm barely past the beginning, and I've already found the videos to be immensely useful. So if you wanted to go into more depth, I really recommend that you check out her videos. You won't regret it.

With that out of the way, let's begin.

So what's a graph? At it's most bare form, a graph is a collection of vertices and edges. If you want to go *really* minimalist, a graph could be simply a collection of vertices. From there, we can connect vertices in any way that is pertinent to the situation at hand.

What I love about graph theory over a lot of other mathematics is that it's *so* visual. This is true for other subjects within mathematics, but you usually have to build up a lot of theory and background before you start seeing those visual connections. For graph theory, on the other hand, things are immediately visual (and can even be helpful in solving the problem), as you can see from a few examples.

![](/images/examples.png)

These are all examples of perfectly valid graphs. Some look strange, but they all represent relationships between the vertices. One thing to note is that we don't care *how* a graph looks, as long as the structure is the same. As such, these two graphs are equivalent, if perhaps a little ugly.

![](/images/graph-equivalence.png)

So if you want to make a graph, you just need to draw some vertices and connect them with various lines. One thing you *cannot* do is have a "hanging" edge. Put differently, every edge has to be capped by a vertex on each side.

Next, a useful property of vertices is what is called the *degree* of a vertex. It's the idea that each vertex has a certain number of connections to it, marked by the edges that go to and from the vertex. Here's a graph with the degree of each vertex.

![](/images/degree.png)

From this, we have a special case. What if *every* vertex has the same degree? More specifically, if any vertex in a specific graph G has a degree of *k*, then we call the graph *k*-regular. I'm introducing this because I want us to tackle a nice problem involving regular graphs.

Lastly, I want to introduce the notion of a *simple* graph. This just means we don't have any loops or "multiple connections" in the graph. I could go on and on about them, but I think a sketch will be more useful.

![](/images/simple-graph.png)

So that's the basics of graph theory, in a *very* brief nutshell. Obviously, there's a lot more to cover, but I wanted to bring these ideas up because we will use them next time to tackle a problem that Dr. Herke in her video series poses, and there's a nice way to visualize the problem that I have found. Stay tuned for that!
