Extra patron attribute needed for Kanopy
----------------------------------------

Whenever a patron logs into an outside service like Kanopy or Hoopla or Lynda.com, that web service talks to our catalog through a connection called SIP2 to verify that the patron has an account and that they are allowed to access their service.  The information that is transmitted across this connection includes some parts of the patron's contact information including the patron's home library.  The problem we have with Kanopy, however, is that, because of the way the receiving end of the Kanopy SIP2 connection is configured, Kanopy cannot determine what the patron's home library is.  Because of this, we need to send the patron's home library through an alternate route.  To make this happen, we've created a new field in the "Permissions" section on a patron's account called "Kanopy (LEAVENWRTH)."

The new "Kanopy (LEAVENWRTH)" permission will have 3 options

- [blank]
- Not allowed
- Allowed (Leavenworth Public Library)

These three options will only be available to staff logged in at LEAVENWRTH in order to prevent staff at other libraries from granting permission to access the Leavenworth Public Library's Kanopy service to their patrons.

This will affect staff and patrons in two ways:

#. When staff at LEAVENWRTH create a new account for a patron, the patron's "Kanopy (LEAVENWRTH)" permission needs to be set to "Allowed (Leavenworth Public Library)" if their home library is LEAVENWRTH or "Not allowed" if their home library is not LEAVENWRTH.  This should happen automatically when a new patron is created.
#. If staff at another library change a patron's home library, staff at LEAVENWRTH will need to update the patron's "Kanopy (LEAVENWRTH)" settings to "Allowed (Leavenworth Public Library)" if the patron's new home library is LEAVENWRTH or"Not allowed" if the patron's new home library is no longer LEAVENWRTH.  This process cannot happen automatically because only LEAVENWRTH staff have access to the "Kanopy (LEAVENWRTH)" permission settings.  Reports will be set up to help LEAVENWRTH staff manage this process.

Creating a new account
----------------------

When logged in at Leavenworth Public Library, click on "Patrons"

.. image:: ../../images/kanopy.leavenwrth.010.png

Then click on the appropriate category on the "New patron" button

.. image:: ../../images/kanopy.leavenwrth.020.png

Then go through your normal process for creating a new patron

.. image:: ../../images/kanopy.leavenwrth.030.png

By default, the patron's home library should be set to LEAVENWRTH and the patron's "Kanopy (LEAVENWRTH)" permission should, by default, be set to "Allowed (Leavenworth Public Library)"

.. image:: ../../images/kanopy.leavenwrth.040.png

If you change the patron's home library from to anything besides LEAVENWRTH, the "Kanopy (LEAVENWRTH)" permission should automatically switch to "Not allowed"

.. image:: ../../images/kanopy.leavenwrth.050.gif

However, if you chage a patron's "Kanopy (LEAVENWRTH)" permission manually, the patron's home library will not update automatically.


Running a report to manually update Kanopy Permission
-----------------------------------------------------
