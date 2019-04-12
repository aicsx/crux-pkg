# crux-pkg

This repo is personal collection of crux pkg.

Steps:
- Modify and add repo in /etc/pkg-get.conf
- Update database repo

```
$ sudo vim /etc/pkg-get.conf

	##
	# /etc/pkg-get.conf
	# pkg-get configuration file

	# package repositories (remote)
	# The first two are remote repoistories, the last is a local one
	pkgdir          /usr/packages/ax|https://raw.githubusercontent.com/aicsx/crux-pkg/master

	# runscripts: if "yes" pre-post install scripts are
	# automatically executed. Handle with care.
	runscripts     yes
	

$ sudo pkg-get sync 
```

You are ok, now can use pkg-get help for other information.

EOF
