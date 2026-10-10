# Exercise 5: Docker Security with AppArmor

Files: app.py, Dockerfile, my-apparmor-profile, apply_apparmor.py, test_restricted_actions.py

Note: this was run on Windows with Docker Desktop. `docker info` shows
SecurityOptions [name=seccomp name=cgroupns] with no apparmor, so the profile
could not be enforced. Both restricted actions returned exit code 0 (not blocked).
On a Linux host with AppArmor enabled the expected exit codes are 1 and 126.
