Names: Laura Wood and Brean Prefontaine

------

I will compile your feedback and scores for the pair project into this document. Please don't alter this document.
Thanks, Danny

------

## Homework assignment 6

Feedback: The poster draft looks good. I think you have the right balance of text and figures so far. Don't neglect to include the way in which you are doing your modeling (i.e., how you set up the field and how the particle trajectories are found). Also, make sure to add your affiliations, etc. Ok, to the problem with the model...I'm pretty sure what you are running into is a scaling issue. Here's what I mean. You've setup the spacing, time step, and even the way in which you do the integration to solve a problem with a small earth with a strong field. When you change things to a big Earth and a small field, the interactions aren't as strong, so solution might involve different scales of spacing and time steps. And you might not see anything if the integration doesn't run for long enough. In computational physics, what we would do is nondimesionalize the problem (https://en.wikipedia.org/wiki/Nondimensionalization) because then there's usall only one or two scales that matter and you can easily control them. So, you have three options: (1) you can spend a bunch of time trying to find the right scale of your other variables to get it to work, (2) you can work to nondimesionalize your problem and figure out the scaling variable (this might not change your work much), or (3) you can leave it and explore the parameter space as you have it (as this model is a proof of principle model). I would suggest given the time you have doing 3 and then talking about 2 in future work. ;) OI'm really glad y'all have gotten this working.

* Score: 20/20

## Homework assignment 5

Feedback: Great questions this week. The poster should be standard size (4 foot by 3 foot). Regarding your modleing the motion of the particle, you are running into a commomn issue in computational physics, which is what is the best way to deal with the interactions. My suggestion would be to calculate the magnetic field where the charge is, update the force, update the velocity, and then update the position. Otherwise you end up with an issue of calculating the field for the whole space, but this leads to arrays nested into a matrix, which can be annoying. Also, it is problematic if your particle leaves the space where you completed the calculation ahead of time because there's no calculated field out there! If you want to try to debug your some aspect of your code this week, I'm happy to help with that. I would suggest that you try to create a more detailed mock up of your poster for this week as it will be the last week for formal feedback.

* Score: 20/20

## Homework assignment 4

Feedback: Things look like they are moving along well. Y'all have a good plan for getting the work done and I think that you have made good progress this week with getting a couple of codes working. I'm not worried about your getting something interesting to present. To answer your questions, the VPython module in jupyter is still a bit buggy. You want to have a "scene" call every time you rerurn your code. The "scene" call draws the window and such, so when you only call it once and then try to update it, it won't do it. It should be as simple as adding scene() to the chunk of code that you update...but I can also help you look at that if it's acting strangely. On top of that, the images that it creates are not figures, they are WebGL animations, so it won't convert them to images, it just returns the object name. You can download the LaTeX instead of the PDF and then screencapture the images in the notebook and place them into the LaTeX file to compile a PDF. There's just not a way around this right now because of the type of animation the VPython code produces...you can switch to matplotlib, but you lose the simple animation aspect.

* Score: 20/20

## Homework Assignment 3

Feedback: I'm really glad to read that y'all are working so closely together. I think from our conversation on Friday I have a much better sense of what you want to do and I think you have a better sense of what the expectations are (so that you aren't trying to do way more than needed). I tihnk you plan to model the motion of particles in a magnetic field is a good starting point and then you can start thinking about structuring the field to map more appropriately to the Earth's field. One thing I noticed in your graphic is that STEVE appears to happen near the Sub-Auroral zone. So if you get the modeling of particles in fields doesn quickly (i.e., next week), then you might be able to extend and compare the Auroral zoe to the sub Auroral zone in your poster to talk about why STEVE is different. Jsut a thought after reading your writeup. Great work this week.

* Score: 20/20

## Homework assignment 2

Feedback: Of course, it's called STEVE...anyway, I think you have laid out an very complete timeline. I'm wondering about STEVE being too much for this project. I don't want to discourage you from pursuing it, but I also don't want this to turn into a Master's thesis project. Perhaps, there's some critical aspects of STEVE that can be modeled, which become obvious fomr your reading. It won't be a problem if your poster talks about STEVE as a phenomenon and then digs into one or two important aspects of STEVE that you model. The reason I'm asking to pump the brakes a little is because it appears that what you might be proposing is a first principles model of STEVE, which I think is a lot more work than I'm asking you to do. In fact, it's probably a pubhlisable results for a reasonably well-known meterological journal. IMO, that's a bit more than I want you to do for this project. So think about what kind of simulation could model some aspects of STEVE (or you can choose the backup plan). Griffth's Ch 11 might be a pretty important starting place for either of them.

* Score 20/20


## Homework assignment 1

Feedback: Laura and Brean, this sounds like a very intersting and cool project. I tihnk you have also already done a fair amount of research into the topic to collect resources that will be helpful. I do worry that you might be biting off a bit more than the project expects as this is not only a project where you would need to model the motion of particles, but also the resulting radiation that they produce. A quick look at some of the resources suggest that these might have come out of master's theses, which is definitely more than I expect for this project. So next week, I'm hoping to see that you have narrowed your ideas down a bit to something tractable given the 7 weeks you have to work on it. Modeling one or another part of this project is fine, so is getting something working that is already been used and talking about how it works. I'm excited to see what you come up with!

* Score: 20/20
