# -*- make -*-
BASE=../..
SUBDIR=vendor/blankon

# Bring in the default rules
include ../../buildlib/defaults.mak

doc binary manpages: sources.list

sources.list: sources.list.in ../../doc/apt-verbatim.ent
	sed -e 's#&blankon-codename;#$(shell ../getinfo blankon-codename)#g' $< > $@
