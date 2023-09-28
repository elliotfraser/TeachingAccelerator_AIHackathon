
# TeachingAccelerator - Power Platform AI Hackathon

This project was my submission to the [2023 Power Platform AI Hack](https://learn.microsoft.com/en-us/events/hack-together-powerplatform-ai/)

__[See my video sumbission HERE](https://www.youtube.com/watch?v=7zHw27HJvbk)__

![Screenshot 2023-09-28 171952](https://github.com/elliotfraser/TeachingAccelerator_AIHackathon/assets/112189810/5d99bce1-2e57-4fe8-bd03-af4a447889c2)

# Problem Statement

*Teachers around the world are spending __1000s of hours__ per year lesson planning for students. __Can we accelerate this with AI?__*

I was originally inspired by this [Teaching with AI Blog](https://openai.com/blog/teaching-with-ai) from OpenAI which is a guide for utilizing ChatGPT for teaching, including prompts for lesson planning. I also spoke with many of my friends who are teachers, some of which were spending __600 hours per year__ planning lessons, for each subject! If we could use AI to accelerate this process even by 20%, it could result in __1000s of work hours saved__ for a school.

# Power Platform Components

My solution consists of the following:
* Model-Driven App
* Custom Pages
* Power Virtual Agents
* Power Automate Flows
* OpenAI ChatGPT API

# Functionality

## Creating a Curriculum

A Curriculum is an array of lessons. To create one using AI, navigate to the Curriculum form, choose a name for this Curriculum, select an Age Group and Subject (these will need to be created if you haven't made some already), and then save the record. Once saved, click the "Ask GPT" button in the command bar. This will launch a Custom Page which has an embedded Power Virtual Agent. 

> Please note, as of 28/09/2023 the, the new PVA component was not working in UK environments, only in US. Hopefully this will be fixed soon.

Context is passed to the chatbot about the record you are working in so there is no need to repeat yourself. The bot will ask you a series of questions as it tries to understand what sort of curriculum you would like. Once satisfied, it will ask you if you would like to export these to the Teaching Accelerator. After selecting yes and closing the bot, you will see all of your lessons have been created along with title and lesson objectives.

![CreateCurriculum](https://github.com/elliotfraser/TeachingAccelerator_AIHackathon/assets/112189810/9bc67eed-2858-4991-82f3-51169c65d4cb)

## Creating a Lesson Plan

Creating lesson plans can be time consuming sometimes taking 30 mins or more to plan. That's a lot of time considering teachers often have 5+ lessons per day! Let's see if we can accelerate this with AI. 

Open one of your lessons and once again, click the "Ask GPT" button in the command bar. A preloaded system message encourages the chatbot to ask you for specific details about your new lesson plan. You are free to let the bot make the decisions for you, explain exactly what you want, or work with the bot to come up with the best lesson plan together. You can even ask the bot to tailor the lesson plan to the specific needs of your class ie by asking for a lesson suitable to those with learning disabilities. 

Once you indicate to the bot that you are satisfied with the lesson plan, it will ask you if you wish to export it to the Teaching Accelerator. On selecting "Yes" and closing the chat, you will see your lesson plan and objective has automatically been uploaded to your lesson record!

![CreatLesson](https://github.com/elliotfraser/TeachingAccelerator_AIHackathon/assets/112189810/fb543603-b73e-4c5c-a208-7cf7d6f505c5)

# Importing

If you'd like to use the Teaching Accelerator yourself or simply see how it's built, please feel free to export from my GitHub and import into your own environment.   

> Please note, as of 28/09/2023 the, the new PVA component was not working in UK environments, only in US. Hopefully this will be fixed soon.

> During the importing process, you will need to provide a valid OpenAI Secret Key. This can be obtained by [creating an account HERE](https://platform.openai.com/overview).

# Future Features

I think there are many ways we can accelerate a teaching by using AI. Not only can we save time but also improve the experience for students. 

For example, some more features I would love to add include:

* AI Creation of homework assignments that can be individualised to the student's abilities and interests.
* A Power Page for students to be assigned and undertake homework tasks.
* A Power Virtual Agent Assistant teacher that can assist students with their work.



