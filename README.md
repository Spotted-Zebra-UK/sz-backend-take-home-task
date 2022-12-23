# Spotted Zebra Backend Take Home Assignment and Pair Programming

We would like to you spend approximately 1 hour in total on the following two tasks:

- Create a small feature in this existing repo
- Create a entity model based on some requirements

In our final meeting we will spend approximately 30 minutes reviewing your feature and ask you to extend it.  We will also spend 10 minutes reviewing your entity model.

## TASK 1: FEATURE IN EXISTING REPO
### Overview
This server contains:

Role Skill Profile Service - used to manage roles and the skills that are required for success in the given role.

Personal Skill Profile Service - used to manage users and thier associated skills.  Each skill associated with a user has a score associated with that user/skill.

Matcher Service - this matches users to roles and calculates the user's score for each role.  The score is calculated using the average of the users skill scores for each skill contained in the Role Skill Profile.


### Prerequisits
npm

nodejs e.g. version 16.13.0 or higher

### Installation

```bash
$ npm install
```

### Running the server

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev
```

### Test

```bash
# unit tests
$ npm run test
```


### Connecting to the server

Once you have started the server, go to the following page in your browser:
http://localhost:3000/

You should see "Hello World!"

Run the matchAll() using:
http://localhost:3000/Matcher/MatchAll

### Your feature task
Complete the method MatcherService->matchAll() which should result in the existing unit tests passing (no change required).

## TASK 2 : ENTITY MODEL

### Your entity model task

Read the below busines requirements.  Create an entity model which represents the information provided.  We are completely flexible as to whether you do this as a drawing that you share with us in the meeting or you 'code' it as part of this repo - whatever is easiest for you.

"Our hiring solution provides managers with a way to identify the skills required for a given role.  We create a skills profile for each role at each company.  Managers can then invite candidates to complete an assessment for that skills profile.  Skills are comprised of traits, a trait is often found in multiple skills.  A candidate’s traits can be measured using tests related to that trait.  For example, Outgoing trait is measured through some questions within the personality tests.   Therefore, depending on what skills are in the skills profile, the candidate may be asked to do one or more tests (e.g. numerical test, personality test).  Scores are saved for each trait and these are rolled up into scores for each skill and a total score for the skills profile.  A report is generated for the candidate for that role, with some content which is based on the skills and score for each skill."
