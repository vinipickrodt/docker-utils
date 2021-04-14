Some docker commands, scripts, tips etc.

# Docker Commands
## Pruning (save disk space + cleaning)

``` docker volume prune ```
Removes all volumes not used by at least one container. (add --force to not ask for confirmation)

> docker system df
* Lists the space used by docker components

TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          29        13        9.444GB   3.499GB (37%)
Containers      16        2         31GB      221.8MB (0%)
Local Volumes   9         9         2.598GB   0B (0%)
Build Cache     153       0         1.565GB   1.565GB


