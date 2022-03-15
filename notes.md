### Domains
All domains will go over a Cloudflare proxy

* basingse.org         -> Nextcloud
* family.basingse.org  -> family documents
* media.basingse.org   -> PhotoPrism
<!-- * portainer.basinge.org   -> Portainer -->
<!-- * admin.basingse.org   -> Nginx Proxy Manager -->
* vault.basingse.org   -> vault warden
* backups.basingse.org -> Raspberry Pi backups with syncthing

* status.basingse.org  -> status page of all services
* start.basingse.org   -> start page with bookmarks
* git.basingse.org     -> private git server ??
* matrix.basingse.org  -> private matrix server ??

* maxgallup.com       -> Home Page with CV
* blog.maxgallup.com  -> Blog Page


### Services
* Backups - syncthing
* Security - fail2ban, pihole, (swag, nginx rev proxy, or traefik), authelia single sign on
* File Sharing - Nextcloud, Photoprism, Samba


### Setup
```
[keizer 12TB RAID 1]  ->  [PiNAS 6TB]
Daily backups to piNAS
```





### Volumes and Containers
* SSD mountpoint `/home/koopa/fast`
* HDD mountpoint `/home/koopa/slow`
* Photoprism Pics+Vids `/home/koopa/slow/media/originals` -> `/photoprism/originals`
* Photoprism Import `/home/koopa/slow/media/import` -> `/photoprism/import`

* container data `/opt/docker`


