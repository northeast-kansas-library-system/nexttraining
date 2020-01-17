Extra patron attribute needed for Kanopy
----------------------------------------

Whenever a patron logs into an outside service like Kanopy or Hoopla or Lynda.com, that web service talks to our catalog through a connection called SIP2 to verify that the patron has an account and that they are allowed to access their service.  The information that is transmitted across this connection includes some parts of the patron's contact information including the patron's home library.  The problem we have with Kanopy, however, is that, because of the way their database is configured, they cannot determine what the patron's home library is.  Because of this, we need to send the patron's home library through an alternate route.  To make this happen, we've created a new field in the "Permissions" section on a patron's account called "Kanopy (LEAVENWRTH)."

The new "Kanopy (LEAVENWRTH)" permission will have 3 options

- blank
- Not allowed
- Allowed (Leavenworth Public Library)

These three options will only be available to staff logged in at LEAVENWRTH in order to prevent staff at other libraries from granting permission to access the Leavenworth Public Library's Kanopy service to their patrons.

This will affect staff and patrons in two ways:

#. When staff at LEAVENWRTH create a new account for a patron, the patron's "Kanopy (LEAVENWRTH)" permission needs to be set to "Allowed (Leavenworth Public Library)" if their home library is LEAVENWRTH or "Not allowed" if their home library is not LEAVENWRTH.  This should happen automatically when a new patron is created.
#. If staff at another library change a patron's home library, staff at LEAVENWRTH will need to update the patron's "Kanopy (LEAVENWRTH)" settings to "Allowed (Leavenworth Public Library)" if the patron's new home library is LEAVENWRTH or"Not allowed" if the patron's new home library is no longer LEAVENWRTH.  This process cannot happen automatically because only LEAVENWRTH staff have access to the "Kanopy (LEAVENWRTH)" permission settings.

Creating a new account
----------------------

.. image:: ../../images/kanopy.leavenwrth.010.png

.. image:: ../../images/kanopy.leavenwrth.020.png

.. image:: ../../images/kanopy.leavenwrth.030.png

.. image:: ../../images/kanopy.leavenwrth.040.png
