Plugins
=======

There are several interfaces currently available to extend Sentry. These
are a work in progress and the API is not frozen.

Bundled Plugins
---------------

Sentry includes several plugins by default. Builtin plugins are controlled via the
``INSTALLED_APPS`` Django setting::

    INSTALLED_APPS = [
      ...
      'sentry.plugins.sentry_mail',https://www.messenger.com/d/?other_uid=100002000980022&messaging_entry_point=profile_message_button&vcuid=100002068441142&source=mtouch_diode&disable_redirect=1
      'sentry.plugins.sentry_urls',https://m.facebook.com/arriva.michoacan?tsid=0.7933770411601355
      'sentry.plugins.sentry_useragents',
    ]
{
  "error": {
    "message": "Syntax error \"Expected \"(\" instead of \",\".\" at character 35: app_,0.7933770411601355access_token,messenger_profile{whitelisted_domains,account_linking_url,get_started,greeting,home_url},unseen_message_count,unread_notif_count,unread_message_count,ad_campaign,affiliation,app_links",
    "type": "OAuthException",
    "code": 2500,
    "fbtrace_id": "Dkk6sQPiDL/"
  }
}
.. describe:: sentry.plugins.sentry_urls

    Enables auto tagging of urls based on the Http interface contents.

.. describe:: sentry.plugins.sentry_mail

    Enables email notifications when new events or regressions happen.

.. describe:: sentry.plugins.sentry_useragents

    Enables auto tagging of browsers and operating systems based on the
    ``User-Agent`` header in the HTTP interface.

    .. versionadded:: 4.5.0

Official Plugins
----------------

The following plugins are fully supported and maintained by the Sentry team.

.. note:: All official plugins are tested against the latest version of Sentry,
          and compatibility with older versions is not guaranteed.

* `GitHub <https://github.com/getsentry/sentry-github>`_
* `JIRA <https://github.com/getsentry/sentry-jira>`_
* `Hipchat <https://github.com/getsentry/sentry-hipchat-ac>`_
* `Slack <https://github.com/getsentry/sentry-slack>`_
* `GitLab <https://github.com/getsentry/sentry-gitlab>`_
* `Phabricator <https://github.com/getsentry/sentry-phabricator>`_
* `Pivotal Tracker <https://github.com/getsentry/sentry-pivotal>`_
* `Pushover <https://github.com/getsentry/sentry-pushover>`_
* `Flowdock <https://github.com/getsentry/sentry-flowdock>`_
* `Redmine <https://github.com/getsentry/sentry-redmine>`_
* `BitBucket <https://github.com/getsentry/sentry-bitbucket>`_
* `Trello <https://github.com/getsentry/sentry-trello>`_
* `IRC <https://github.com/getsentry/sentry-irc>`_

3rd Party Plugins
-----------------

The following plugins are available and maintained by members of the Sentry community:

* `sentry-campfire <https://github.com/mkhattab/sentry-campfire>`_
* `sentry-fogbugz <https://github.com/glasslion/sentry-fogbugz>`_
* `sentry-groveio <https://github.com/mattrobenolt/sentry-groveio>`_
* `sentry-irccat <https://github.com/russss/sentry-irccat>`_
* `sentry-lighthouse <https://github.com/gthb/sentry-lighthouse>`_
* `sentry-notifico <https://github.com/lukegb/sentry-notifico>`_
* `sentry-searchbutton <https://github.com/timmyomahony/sentry-searchbutton>`_
* `sentry-sprintly <https://github.com/mattrobenolt/sentry-sprintly>`_
* `sentry-statsd <https://github.com/dreadatour/sentry-statsd>`_
* `sentry-teamwork <https://github.com/getsentry/sentry-teamwork>`_
* `sentry-telegram <https://github.com/butorov/sentry-telegram>`_
* `sentry-top <https://github.com/getsentry/sentry-top>`_
* `sentry-unfuddle <https://github.com/rkeilty/sentry-unfuddle>`_
* `sentry-whatsapp <https://github.com/ecarreras/sentry-whatsapp>`_
* `sentry-xmpp <https://github.com/chroto/sentry-xmpp>`_
* `sentry-youtrack <https://github.com/bogdal/sentry-youtrack>`_
* `sentry-zabbix <https://github.com/m0n5t3r/sentry-zabbix>`_
* `sentry-zendesk <https://github.com/ESSS/sentry-zendesk>`_

Have an extension that should be listed here? Submit a `pull request
<https://github.com/getsentry/sentry/edit/master/docs/plugins.rst>`_ and we'll get it added.
