# Laminar CI scripts

This is but a collection of build scripts that I use together with Laminar, a fully scriptable CI/CD solution that you can bend to your will with a lil' bit of scripting.

Here are a few "fun things" about this:

1. Scripts are run by their shebang; meaning, those scripts could also be `#!/usr/bin/env node` to make JavaScript jobs.
2. YOU - or, I - are responsible for triggering those runs. So I have to figure out a nice cron-ish way to track remote changes and then run them. To specify a reason, set `LAMINAR_REASON` and pass parameters, which then become environment variables in the script.

And, everything is technically shared. In the future, I will want to run this in either a container or VM for better isolation. Right now, a basic chroot will have to suffice...

## Why post them in the public?

Cuz why not. o.o
