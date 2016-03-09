Notes for the 'European septic shock' cohort manuscript
Currently just doing a copy/paste job into the document.txt file from the results.md in the src git submodule

## inbox.todo

Running list of tasks, but transfer these to the [issue tracker](https://github.com/docsteveharris/paper-euroepi/issues) (and then remove from here)

- descriptive stuff to report
    + sofa.24
    + rx.roids
    + pmh.betablocker
    + ne.24
    + lactate
    + first 24 hour fluid resus
    + pathology 

## now.todo

- add in Morelli inclusion criteria
    + septic shock plus heart rate > 95 and 'high dose' norad to maintain MAP > 65 for 24 hours
        * not done this: kept all regardless of heart rate
- CONSORT flow diagram as per Morelli
    + drop if off NAd by 24 hours (n=51) 
        + dropping where NAd <0.1 - but lose 40% sample ?revise
    + present a similar comparison
        * inclusion were that NAd still required at 24 hrs
        * exclus

# Notes

## Log

### 2016-03-08

- done the strobe diagram
- tidied table 1
- started results text

## Robi and Sara's original precis

    - evaluate what is the mortality in septic shock patients throughout Europe

Agreed. We seem to be doing this.

    - evaluate if differences in outcome among ITU can be related to different managements in term of sedation, fluid filling, inotrops ( global severity seems to be similar in the 8 centers, they are all general ITU with surgical+medical+/- trauma pts)

Good. See to above - have included this, but in essence we will examine the importance of the 'hospital/centre' effect after adjusting for important practice parameters. Practically, we will build a model to predict 24 hour noradrenaline dose  (?log transformed with an adjustment for 'zero' doses) at 24h controlling for patient characteristics at baseline and assess the intra-class correlation (for patients nested within hospital). Then repeat this after including the 'practice parameters'.

    - evaluate if different HR ( ≥95 or less) in patients that receive same amount of NE is related with different outcome( so if tachycardic patients die more than pts with normal HR at same level of NE)

You're asking here if heart rate (tachy, tachy>95) has an independent effect on outcome after adjusting for Norad dose. Happy to look at this but I am fairly sure the answer will be 'yes' because HR is _always_ assocaited with worse outcomes in models.



## Morelli paper

Morelli A, Ertmer C, Westphal M, Rehberg S, Kampmeier T, Ligges S, et al. Effect of Heart Rate Control With Esmolol on Hemodynamic and Clinical Outcomes in Patients With Septic Shock. JAMA. 2013 Oct 23;310(16):1683–9. 

- inclusion: 24 hours of 'optimisation' before enrollment that included CVP >= 8 and PAOP >= 8 and peristing requirement for Norad for MAP > 65
- exclusion:
    + prior beta-blocker therapy
    +   heart rate > 95 at 24 hours
    + <18yrs
- intervention continued for 96 hours


Patient characteristics at baseline (randomisation event which is 24 hours post-resus)

- mean age 65ish
- 70% male
- BMI 30ish
- fluid in pre-ranodomisation approx 5l
- fluid in approx 4-5l/day for 1st 96 hours

# Do not read

Well, you can if you want, but I wouldn't recommend it

## Technical repo management notes

Note that there are two remotes specified
- github: to use for project management features
- penflip: to use for collaborative writing

And there's a submodule for code which I can keep up to date, but then re-use elsewhere (for example, if we decide to work on a second paper).
