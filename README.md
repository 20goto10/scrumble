scrumble
========

A simple Google hangout app that links a Hangout to hipchat.

The original purpose of Scrumble was to randomize the order of presenters for 
a collaborative team. However, it seemed excessive to make all the users
load Scrumble to see the presenter order, and our team wound up copying
the randomized order into a Hipchat window. 

Now, Scrumble takes the list of users and can randomize it and send it
to a given Hipchat room. It can also send an alert to the room, which
includes text and an image with a link to the Hangout. Non-Hangouts users can
still send the randomized presenter order with a text copy and paste.

The Hipchat room, API key, and alert image are all saved to the user's
cookies, and preserved for 30 days after use. 

The Hipchat features require the scrum participants to have a Hipchat room,
and Scrumble requires the main user to have a Hipchat API key capable of
sending to that room. 

Getting it Working
==================

If you obtain Scrumble, you'll need to do a bit of manipulation to get it
running under Hangouts. You'll need to set up a Google hangouts
developer API key and build a project under it that links to someplace
you've got the scrumble.xml file available via HTTP.   

More information on creating Hangout apps, including deployment info, is located here:
https://developers.google.com/+/hangouts/writing

Craziness
=========

Believe it or not, there's no Hangout API interface for connecting to
gchat. That seems crazy. 

ROADMAP
=======
- User exclusion list [checkboxes to allow some users to not be listed
  in the roster, or always be first]
- handler for users who join late (append their names to the listed Scrumble users and auto-send to Hipchat?)
- Manual user reordering and save?
- Make available to non-dev public as an "official" Google app
- suggestions welcome!

WORKING
=======
- save cookies on change to any field
- "alarm" includes link to Hangout
- "alarm" image and thumbnail
- Hipchat messaging
- cookie preservation
- user randomization
