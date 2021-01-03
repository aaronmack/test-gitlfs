## Test GitLFS
This is a project for test git-lfs

## Prepare

```bash
scoop install git-lfs
```

## Git-LFS Examples

```bash
Examples
--------

* List the patterns that Git LFS is currently tracking:

    git lfs track

* Configure Git LFS to track GIF files:

    git lfs track "*.gif"

* Configure Git LFS to track PSD files and make them read-only unless locked:

    git lfs track --lockable "*.psd"

* Configure Git LFS to track the file named project [1].psd:

    git lfs track --filename "project [1].psd"
```

## Resources

### How to add a single file to GIT LFS?
*https://stackoverflow.com/questions/51898857/how-to-add-a-single-file-to-git-lfs*

## How to

```bash
git lfs track --filename TEST-BIG-FILE-UE4Game.exe
```

### Find Big files

```bash
# Run follows command in the cygwin bash
find -type f -exec du -Sh {} + | sort -rh | head -n 5
```