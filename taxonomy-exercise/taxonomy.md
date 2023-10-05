Property taxonomy exercise 
====

This exercise is meant to show a command of the technologies we use, as well as a keen head for problem solving and
tackling abstract challenges. We ask to have the challenge returned within **three days** of it being assigned.

It should take approximately 3 hours to finish this task, but let us know if you need more time. 

The task is divided into two parts, the first meant to challenge you to show API skills and backend system design while
the second is a small Frontend task to evaluate how well you can consume the API you have just created in a good way.

Feel free to use the technology/framework you are the most comfortable with (big plus if any of it includes PHP/Laravel/Vue.js!).

If you do not have time to finish the task, please leave comments describing how you would have implemented the missing
parts.

# Part One 

In the PropTech business we need to model the relationships between corporations, buildings and properties 
(rental units) so that we can accurately reflect reality and give our customers a structure they feel comfortable 
relating to. This structure ("taxonomy" if you will) is what you will be modeling in the first part of this challenge!

We have our root node (only one, representing the Corporation) and several child nodes.
Each of these nodes may have its own children. 

It can be structured as something like this: 
```
        root
       /    \
      a      b
      |
      c
    / 	\
   d     e
```

## We need 3 endpoints that will serve basic operations : 

0. Add a new node to the tree.
1. Get all child nodes of a given node from the tree (only 1 layer of children).
2. Change the parent node of a given node, with one rule: a Building node cannot have a Property node as parent.

Each node should have the following data: 

0. Node identifier.
1. Node name.
2. Relationship to the parent node.
3. The height of the node (in the example above `height(root)=0` and `height(a)=1`).
4. The nodes should have a type from the following list: Corporation, Building, Property.
4. Buildings should have an extra field specifying the zip code they are located in.
5. Properties should have an extra field specifying the monthly rent of the property.

# Part Two

Now that you have an API to work with, let's create a quick and dirty UI we can use to move properties around.

### We need two things:

0. A view that shows the hierarchy (can be absolutely quick and dirty).
1. A feature that allows us to move a Property node from one Building node to another by calling the "change parent node" endpoint.

A few notes:

0. Bonus points if each node is represented by an independent UI component.
1. Good structure is more important than styling (don't be afraid to go ugly, as long as your code is sound!)

# How to hand it in

Please upload your solution to a git repository (BitBucket, GitLab or GitHub) and provide a README.md file with 
documentation, including how to run your solution, then send us a link to the repo (make sure it's public or otherwise
accessible).

Feel free to describe what you would have improved in your solution if more time was given!


