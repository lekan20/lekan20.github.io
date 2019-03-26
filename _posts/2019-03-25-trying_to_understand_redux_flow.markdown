---
layout: post
title:      "Trying to understand Redux Flow"
date:       2019-03-26 00:02:43 +0000
permalink:  trying_to_understand_redux_flow
---


Redux flow has give me a lot of trouble to understand. It feels like such an abstract topic to me that I want to use this post to help me understand it more. 

Redux Flow has three parts

1. Action
2. Reducer 
3. Updated State

The **Action** or action.type tells us what we’re looking to do. If we have a state of {count: 0} and want to increase it by one our action will have a type of that tells it to increase the count {type: ‘INCREASE_COUNT”}.

The **Reducer** is a combination of the current state and the action. Reducers are pure functions so you’re not going to manipulate the current state in the reducer. It’ll create a new state from the current state. In our example if the INCREASE_COUNT action has the reducer increase the count by one, it’ll create a new state using the current_state and adding 1 to it. It returns a Javascript object we’ll use for the **Updated State**. 

It feels so simple to me writing it here but implementing it has been hard. I've felt that way with a lot of concepts. I know I need to practice these and write code try work through them but I feel it's hard to find activities to do. I'll leave writing this feeling that I have a solid grasp but I know when I need to explain it or write new code on it I'll struggle. 

Even saying that, revisting the lessons and reading additonal resources (https://redux.js.org/basics/basic-tutorial) helped me understand this a lot more than I did 5 weeks ago. I know it's a cumulitive effort of all of it rather than me finding one magical source that explains it ot me in a way that it clicks. Each time I read something or try something else the picture gets clearer in my head. 

