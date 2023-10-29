.. Pegasus documentation master file, created by
   sphinx-quickstart on Mon Mar 18 15:47:15 2019.

Partly's documentation
===============

Note: Most of the things in this doc site are specific to SaaS Pegasus, and some of it isn't relevant to Partly

That's the starter template that we built the initial product with here at Partly. Over time we'll add to this documentation rather than starting from scratch. Note that not all parts of this documentation are relevant. For example, we use:
* Docker installation (not python or any virtualenv stuff)
* Tailwind (no other css)
* Alpine / HTMX
* Waffle for feature flags
* Celery
* Teams
* Not stripe (stripe is in the partly app, but doesn't use dj-stripe)

**To see Partly specific stuff, look at the top of the left sidebar.**

---

Here you'll find everything you need to know about setting up and configuring Pegasus for your project.

You'll need a Pegasus license to proceed.
If you don't have one, head on over to `saaspegasus.com`_ to get yours.

If you're just getting started, you'll want to start with the :doc:`getting-started` guide.

The source for this documentation can be `found on Github <https://github.com/czue/pegasus-docs/>`_ and
contributions are most welcome!

.. toctree::
   :maxdepth: 2

   partly-faq
   getting-started
   customizations
   configuration
   code-structure
   using-virtualenvs
   front-end
   css
   page-metadata
   docker
   teams
   subscriptions
   payments
   forms
   apis
   internationalization
   wagtail
   flags
   celery
   async
   deployment
   github-actions
   cookbooks
   upgrading
   release-notes

.. _saaspegasus.com: https://www.saaspegasus.com/
