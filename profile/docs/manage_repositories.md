# ros-event-camera repository management

## New release of existing repositories

Assuming you are in your workspace and suppose you want to create a new release of ``metavision_driver`` for distro Humble that captures the changes in ``master``:
```bash
my_repo=metavision_driver
cd src/${my_repo}
# make sure the master is up-to date
git checkout master && git pull
# look that every thing is committed
git status
# checkout the humble branch
git checkout humble && git pull
# apply the latest changes from master to humble
git rebase master
# generate the changelog
catkin_generate_changelog
# edit the CHANGELOG.rst file, save it, and COMMIT(!) it
git commit -a
# bump the package version, create tags etc
catkin_prepare_release
# push the updates to the release repository
bloom-release --rosdistro humble ${my_repo}
```
Now to release the identical thing to e.g. Rolling:
```bash
git checkout rolling
git rebase humble
git push -u origin rolling
bloom-release --rosdistro rolling ${my_repo}
```
