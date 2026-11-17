# codeprospecialist.github.io

Static site served at https://codeprospecialist.github.io

## Layout

    index.html          Plain landing page. Deliberately does not list the
                        apps: each app's pages stand alone, so someone who
                        arrives from one app's Play listing is not routed
                        toward the others.

    app-ads.txt         One file for every app, and it has to stay at the
                        root because that is the only place crawlers look.
                        It authorises the AdMob publisher account, not an
                        individual app, so one line covers everything.
                        Add a line per extra ad network, not per app.

    fennarith/          One folder per app, self-contained.
      index.html
      privacy.html      The URL that goes in that app's Play listing.

## Adding an app

Copy the fennarith folder, rename it, rewrite both pages, and paste the new
privacy URL into that app's Play Console listing. Nothing at the root needs
changing unless a new ad network is involved.

Each app needs its own privacy policy rather than a shared one. Fennarith's
says the maths never leaves the phone, which will not be true of an app that
syncs, and a policy that overstates is worse than no policy.
