---
title: "Data Assets and Scriptable Objects as First Stepping Stones toward Data Oriented Development"
description: I explain how nice it is to empower our designers and artists by getting fed on data.
date: 2025-05-06T12:21:27-04:00
categories:
    - Technical Explanation
tags: 
    - Quickly Explained
    - Unity
    - Unreal
    - Data Oriented
image: 
math:
license:
hidden: false
comments: true
draft: false
---

## How the usage DA/SO can help your development process

I frequently use [Scriptable Objects](https://docs.unity3d.com/6000.0/Documentation/Manual/class-ScriptableObject.html) in Unity and [Data Assets](https://dev.epicgames.com/documentation/en-us/unreal-engine/data-assets-in-unreal-engine) in Unreal to help the design team.

Essentially, instead of telling them to modify some variable in the
code, I tell them to modify some variable in a specific file, either the
DA or SO.

It's nice for them because :
 * It's way **simpler**.
 * All related data are **bundle** together.
 * They can make "backups" of the file in order to **test new things**
 and safely come back to the previous values.

It's nice for me because I can focus on **developing new systems**, and I can
easily make changes to the codebase **without worrying** about the designers
getting lost after all that Friday night refactoring.

My workflow goes on like this :
- First, I program the system.
- Then, I abstract the data used into a DA/SO.
- Finally, I explain to the designer where is the new DA/SO and what it is
responsible for.

It's simple, and can have many advantages even for the **gameplay itself**.
For example, you might want to have an easy or hard mode. Just make an
easy and a hard SO/DA. Just feed the right data.

In that regard, I think it is a good first step into data driven gameplay,
by enabling designers and artists to customize gameplay elements
just by changing data.
