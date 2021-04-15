Some docker commands, scripts, tips etc.

# Docker Commands
## Pruning (Release unused disk space on Windows 10)

1. > docker system df
* Lists the space used by docker components
```
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          29        13        9.444GB   3.499GB (37%)
Containers      16        2         31GB      221.8MB (0%)
Local Volumes   11        9         27.55GB   24.95GB (90%)
Build Cache     153       0         1.565GB   1.565GB
```

2. > docker volume prune
* Removes all volumes not used by at least one container. (add --force to not ask for confirmation)

3. > wsl --shutdown
* Stop WSL to release the VHDX file.

4. > Optimize-VHD -Path "C:\Users\vinip\AppData\Local\Docker\wsl\data\ext4.vhdx" -Mode Full
* Releases the unused space from VHDX filesystem.

