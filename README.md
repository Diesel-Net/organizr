# organizr
Organizr https://github.com/causefx/Organizr


docker create \
  --name=organizr \
  -v <path to data>:/config \
  -e PGID=<gid> -e PUID=<uid>  \
  -p 80:80 \
  -e fpm="false" \ # optional
  -e branch="v2-master" \ # optional
  organizr/organizr
