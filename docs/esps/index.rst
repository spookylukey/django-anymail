.. _supported-esps:

Supported ESPs
==============

Anymail currently supports these Email Service Providers.
Click an ESP's name for specific Anymail settings required,
and notes about any quirks or limitations:

.. these are listed in alphabetical order

.. toctree::
   :maxdepth: 1

   mailgun
   mandrill
   postmark
   sendgrid


Anymail feature support
-----------------------

The table below summarizes the Anymail features supported for each ESP.

.. currentmodule:: anymail.message

======================================    ====================== ======================= ======================= =======================
Email Service Provider                    :ref:`mailgun-backend` :ref:`mandrill-backend` :ref:`postmark-backend` :ref:`sendgrid-backend`
======================================    ====================== ======================= ======================= =======================
.. rubric:: :ref:`Anymail send options <anymail-send-options>`
----------------------------------------------------------------------------------------------------------------------------------------
:attr:`~AnymailMessage.metadata`          Yes                    Yes                     No                      Yes
:attr:`~AnymailMessage.send_at`           Yes                    Yes                     No                      Yes
:attr:`~AnymailMessage.tags`              Yes                    Yes                     Max 1 tag               Yes
:attr:`~AnymailMessage.track_clicks`      Yes                    Yes                     No                      Yes
:attr:`~AnymailMessage.track_opens`       Yes                    Yes                     Yes                     Yes

.. rubric:: :ref:`Status <esp-send-status>` and tracking
----------------------------------------------------------------------------------------------------------------------------------------
:attr:`~AnymailMessage.anymail_status`    Yes                    Yes                     Yes                     Yes
======================================    ====================== ======================= ======================= =======================


.. Status tracking webhooks                  (coming)               (coming)                (coming)                (coming)
.. .. rubric:: :ref:`inbound`
.. ----------------------------------------------------------------------------------------------------------------------------------------
.. Inbound webhooks                          (coming)               (coming)                (coming)                (coming)

Trying to choose an ESP? Please **don't** start with this table. It's far more
important to consider things like an ESP's deliverability stats, latency, uptime,
and support for developers. The *number* of extra features an ESP offers is almost
meaningless. (And even specific features don't matter if you don't plan to use them.)


Other ESPs
----------

Don't see your favorite ESP here? Anymail is designed to be extensible.
You can suggest that Anymail add an ESP, or even contribute
your own implementation to Anymail. See :ref:`contributing`.