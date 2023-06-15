# Comparing `tmp/invenio-communities-6.7.0.tar.gz` & `tmp/invenio-communities-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-communities-6.7.0.tar", last modified: Wed Jun  7 08:24:53 2023, max compression
+gzip compressed data, was "dist/invenio-communities-7.0.0.tar", last modified: Thu Jun 15 11:49:07 2023, max compression
```

## Comparing `invenio-communities-6.7.0.tar` & `invenio-communities-7.0.0.tar`

### file list

```diff
@@ -1,648 +1,657 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/.prettierrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/administration/communities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/90642d415317_create_communities_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/api.js
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/GroupsApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/UsersApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/CommunityTypeLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/context.js
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/context.js
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/index.js
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/appUrls.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)   130749 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/dumpers/featured.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/entity_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v1/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v2/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/v7/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/systemfields/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/records/systemfields/pidslug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/resources/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/resources/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/communities/services/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/communities/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/fixtures/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/fixtures/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/members/services/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    24918 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/members/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/notifications/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/records/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/records/records/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/searchapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_details.html
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_search.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/access-status-label.html
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities/views/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/views/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/views/communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/views/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/views/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/invenio_communities/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/invenio_communities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 08:24:52.000000 invenio-communities-6.7.0/invenio_communities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/run-js-linter.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_community_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_relations_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_relations_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29959 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/communities/tests_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/members/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/members/test_members_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/members/test_members_no_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/members/test_members_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    34168 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/members/test_members_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/jsonschemas/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/jsonschemas/mocks/mock-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v6/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v6/mocks/mock-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:24:53.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v7/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/mappings/v7/mocks/mock-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/records/test_mockrecords_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-07 08:24:42.000000 invenio-communities-6.7.0/tests/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.prettierrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/administration/communities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/02cd82910727_update_role_id_type_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/37b21951084c_update_role_id_type_downgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/90642d415317_create_communities_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/GroupsApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/UsersApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/CommunityTypeLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/appUrls.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130749 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cache/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/dumpers/featured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/entity_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/pidslug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/fixtures/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/fixtures/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/notifications/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/searchapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/access-status-label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32162 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/run-js-linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/cache/test_identity_redis_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_community_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_relations_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_relations_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29959 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/tests_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_no_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34235 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/mocks/mock-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/mocks/mock-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/mocks/mock-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/test_mockrecords_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/test_notifications.py
```

### Comparing `invenio-communities-6.7.0/.editorconfig` & `invenio-communities-7.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/.tx/config` & `invenio-communities-7.0.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/AUTHORS.rst` & `invenio-communities-7.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/CHANGES.rst` & `invenio-communities-7.0.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,22 @@
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 
 Changes
 =======
 
+Version 7.0.0 (released 2023-06-15)
+-----------------------------------
+
+- cache: adds unmanaged groups to be cached and loaded in the identity
+- adds identity cache
+- add groups as community members
+- assets: display metrics on deletion modal
+
 Version 6.7.0 (released 2023-06-07)
 -----------------------------------
 
 - notifications: add member recipient generator
 - tests: add notification member recipient generator test case
 - services: add extra_filter param
 - services: provide explicit scan params
```

### Comparing `invenio-communities-6.7.0/CONTRIBUTING.rst` & `invenio-communities-7.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/LICENSE` & `invenio-communities-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/MANIFEST.in` & `invenio-communities-7.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/PKG-INFO` & `invenio-communities-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-communities
-Version: 6.7.0
+Version: 7.0.0
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-communities
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,22 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 7.0.0 (released 2023-06-15)
+        -----------------------------------
+        
+        - cache: adds unmanaged groups to be cached and loaded in the identity
+        - adds identity cache
+        - add groups as community members
+        - assets: display metrics on deletion modal
+        
         Version 6.7.0 (released 2023-06-07)
         -----------------------------------
         
         - notifications: add member recipient generator
         - tests: add notification member recipient generator test case
         - services: add extra_filter param
         - services: provide explicit scan params
```

### Comparing `invenio-communities-6.7.0/README.rst` & `invenio-communities-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/docs/Makefile` & `invenio-communities-7.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/docs/conf.py` & `invenio-communities-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/docs/index.rst` & `invenio-communities-7.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/docs/make.bat` & `invenio-communities-7.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/administration/communities.py` & `invenio-communities-7.0.0/invenio_communities/administration/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py` & `invenio-communities-7.0.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/alembic/90642d415317_create_communities_branch.py` & `invenio-communities-7.0.0/invenio_communities/alembic/90642d415317_create_communities_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py` & `invenio-communities-7.0.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py` & `invenio-communities-7.0.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py` & `invenio-communities-7.0.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py` & `invenio-communities-7.0.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from sqlalchemy.dialects import mysql, postgresql
 from sqlalchemy_utils import JSONType, UUIDType
 
 # revision identifiers, used by Alembic.
 revision = "fbe746957cfc"
 down_revision = "f701a32e6fbe"
 branch_labels = ()
-depends_on = None
+depends_on = (
+    "a14fa442680f",
+    "2f63be7b7572",
+)  # where the accounts_role and request_metadata table are created
 
 
 def upgrade():
     """Upgrade database."""
     op.add_column(
         "communities_members", sa.Column("active", sa.Boolean(), nullable=False)
     )
```

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,15 @@
     Image,
     withCancel
 } from "react-invenio-forms";
 import {
     Dropdown,
     List
 } from "semantic-ui-react";
+import _truncate from "lodash/truncate";
 
 export class MembersSearchBar extends Component {
     constructor(props) {
         super(props);
 
         this.state = {
             isFetching: false,
@@ -98,16 +99,22 @@
                         group.links.avatar
                     }
                     avatar / >
                     <
                     List.Content >
                     <
                     List.Header as = "a" > {
-                        group.id
+                        group.name
                     } < /List.Header> <
+                    List.Description > {
+                        _truncate(group.description, {
+                            length: 30
+                        })
+                    } <
+                    /List.Description> <
                     /List.Content> <
                     /List.Item> <
                     /List>
                 ),
             };
         });
     };
@@ -145,15 +152,15 @@
         const serializedSelectedMember = {
             id: newSelectedMember.id,
             type: searchType,
             avatar: newSelectedMember?.links?.avatar,
         };
 
         if (searchType === "group") {
-            serializedSelectedMember["name"] = newSelectedMember.id;
+            serializedSelectedMember["name"] = newSelectedMember.name; // The schema will pass the id if the name is missing
         } else {
             serializedSelectedMember["name"] = this.serializeMemberName(newSelectedMember);
         }
         selectedMembers[serializedSelectedMember.id] = serializedSelectedMember;
         handleChange(selectedMembers);
     };
```

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -160,15 +160,15 @@
             } >
             <
             b className = "mr-10" > {
                 result.member.name
             } < /b>
 
             {
-                result.member.is_group && ( <
+                result.member.type === "group" && ( <
                     Label className = "mr-10" > {
                         i18next.t("Group")
                     } < /Label>
                 )
             } {
                 result.is_current_user && ( <
                     Label className = "primary" > {
```

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -47,15 +47,15 @@
             Item.Header className = {
                 !result.member.description ? "mt-5" : ""
             } >
             <
             b > {
                 result.member.name
             } < /b> {
-                result.member.is_group && ( <
+                result.member.type === "group" && ( <
                     Label className = "ml-10" > {
                         i18next.t("Group")
                     } < /Label>
                 )
             } <
             /Item.Header> {
                 result.member.description && ( <
```

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -11,67 +11,108 @@
 } from "@translations/invenio_communities/i18next";
 import React, {
     Component
 } from "react";
 import {
     Button,
     Icon,
+    Loader,
     Modal,
     Message,
     Grid,
     Checkbox,
-    Input
+    Input,
 } from "semantic-ui-react";
 import PropTypes from "prop-types";
 import {
     Trans
 } from "react-i18next";
 import {
     communityErrorSerializer
 } from "../../api/serializers";
 import {
     ErrorMessage,
+    http,
     withCancel
 } from "react-invenio-forms";
 
 export class DeleteCommunityModal extends Component {
     constructor(props) {
         super(props);
         this.INITIAL_STATE = {
             modalOpen: false,
-            loading: false,
+            loading: true,
             checkboxMembers: false,
             checkboxRecords: false,
             checkboxSlug: false,
             inputSlug: "",
             error: undefined,
         };
         this.checkboxRef = React.createRef();
         this.openModalBtnRef = React.createRef();
         this.state = this.INITIAL_STATE;
     }
 
+    componentDidMount() {
+        this.updateCommunityMetrics();
+    }
+
     componentDidUpdate(prevProps, prevState) {
         const {
+            loading,
             modalOpen
         } = this.state;
-        if (modalOpen && modalOpen !== prevState.modalOpen) {
+        if (!loading && modalOpen && modalOpen !== prevState.modalOpen) {
             const {
                 current: {
                     inputRef
                 },
             } = this.checkboxRef;
             inputRef.current.focus();
         }
     }
 
     componentWillUnmount() {
         this.cancellableDelete && this.cancellableDelete.cancel();
+        this.cancellableMembersCountFetch && this.cancellableMembersCountFetch.cancel();
+        this.cancellableRecordsCountFetch && this.cancellableRecordsCountFetch.cancel();
     }
 
+    updateCommunityMetrics = async () => {
+        this.setState({
+            loading: true
+        });
+        const {
+            community
+        } = this.props;
+        this.cancellableMembersCountFetch = withCancel(http.get(community.links.members));
+        this.cancellableRecordsCountFetch = withCancel(http.get(community.links.records));
+
+        try {
+            const membersResponse = await this.cancellableMembersCountFetch.promise;
+            const recordsResponse = await this.cancellableRecordsCountFetch.promise;
+            this.setState({
+                loading: false,
+                membersCount: membersResponse.data.hits.total,
+                recordsCount: recordsResponse.data.hits.total,
+            });
+        } catch (error) {
+            console.error(error);
+            const {
+                message
+            } = communityErrorSerializer(error);
+            if (message) {
+                this.setState({
+                    error: message,
+                    loading: false
+                });
+            }
+        }
+    };
+
     handleInputChange = (event) => {
         this.setState({
             inputSlug: event.target.value
         });
     };
 
     handleCheckboxChange = (e, {
@@ -106,15 +147,21 @@
     };
 
     openConfirmModal = () => this.setState({
         modalOpen: true
     });
 
     closeConfirmModal = () => {
-        this.setState(this.INITIAL_STATE);
+        let {
+            loading
+        } = this.state;
+        this.setState({
+            ...this.INITIAL_STATE,
+            loading: loading
+        });
         this.openModalBtnRef?.current?.focus();
     };
 
     handleDelete = async () => {
         this.setState({
             loading: true
         });
@@ -152,14 +199,16 @@
             modalOpen,
             loading,
             error,
             checkboxMembers,
             checkboxRecords,
             checkboxSlug,
             inputSlug,
+            membersCount,
+            recordsCount,
         } = this.state;
         const {
             label,
             community
         } = this.props;
         const communitySlug = community.slug;
         return ( <
@@ -195,182 +244,195 @@
             onClose = {
                 this.closeConfirmModal
             }
             size = "tiny" >
             <
             Modal.Header > {
                 i18next.t("Permanently delete community")
-            } < /Modal.Header> <
-            Modal.Content >
-            <
-            Trans >
-            Are you < strong > absolutely sure < /strong> you want to delete the community? <
-            /Trans> <
-            /Modal.Content> <
-            Modal.Content >
-            <
-            Message negative >
-            <
-            Message.Header >
-            <
-            Grid columns = {
-                2
-            }
-            verticalAlign = "middle" >
-            <
-            Grid.Column width = {
-                1
-            } >
-            <
-            Icon name = "warning sign" / >
-            <
-            /Grid.Column> <
-            Grid.Column width = {
-                15
-            } > {
-                i18next.t("This action CANNOT be undone!")
-            } <
-            /Grid.Column> <
-            /Grid> <
-            /Message.Header> <
-            Message.Content >
-            <
-            Checkbox id = "members-confirm"
-            ref = {
-                this.checkboxRef
-            }
-            label = {
-                /* eslint-disable-next-line jsx-a11y/label-has-associated-control */
-                <
-                label >
-                <
-                Trans >
-                <
-                strong > All the members < /strong> will be removed from the
-                community. <
-                /Trans> <
-                /label>
-            }
-            checked = {
-                checkboxMembers
-            }
-            onChange = {
-                this.handleCheckboxChange
-            }
-            /> <
-            Checkbox id = "records-confirm"
-            label = {
-                /* eslint-disable-next-line jsx-a11y/label-has-associated-control */
-                <
-                label >
-                <
-                Trans >
-                <
-                strong > All the records < /strong> will be removed from the
-                community. <
-                /Trans> <
-                /label>
-            }
-            checked = {
-                checkboxRecords
-            }
-            onChange = {
-                this.handleCheckboxChange
-            }
-            /> <
-            Checkbox id = "slug-confirm"
-            label = {
-                /* eslint-disable-next-line jsx-a11y/label-has-associated-control */
-                <
-                label >
-                <
-                Trans >
-                You < strong > CANNOT < /strong> reuse the community identifier " {
-                    {
-                        communitySlug
+            } < /Modal.Header> {
+                loading && < Loader active = {
+                    loading
+                }
+                />} <
+                Modal.Content >
+                    <
+                    Trans >
+                    Are you < strong > absolutely sure < /strong> you want to delete the community? <
+                    /Trans> <
+                    /Modal.Content> <
+                    Modal.Content >
+                    <
+                    Message negative >
+                    <
+                    Message.Header >
+                    <
+                    Grid columns = {
+                        2
                     }
+                verticalAlign = "middle" >
+                    <
+                    Grid.Column width = {
+                        1
+                    } >
+                    <
+                    Icon name = "warning sign" / >
+                    <
+                    /Grid.Column> <
+                    Grid.Column width = {
+                        15
+                    } > {
+                        i18next.t("This action CANNOT be undone!")
+                    } <
+                    /Grid.Column> <
+                    /Grid> <
+                    /Message.Header> <
+                    Message.Content >
+                    <
+                    Checkbox
+                id = "members-confirm"
+                ref = {
+                    this.checkboxRef
                 }
-                ". <
-                /Trans> <
-                /label>
-            }
-            checked = {
-                checkboxSlug
-            }
-            onChange = {
-                this.handleCheckboxChange
-            }
-            /> <
-            /Message.Content> <
-            /Message> <
-            /Modal.Content> <
-            Modal.Content >
-            <
-            Trans >
-            Please type < strong > {
-                {
-                    communitySlug
-                }
-            } < /strong> to confirm. <
-            /Trans> <
-            Input fluid value = {
-                inputSlug
-            }
-            onChange = {
-                this.handleInputChange
-            }
-            /> <
-            /Modal.Content> <
-            Modal.Actions > {
-                error && ( <
-                    ErrorMessage header = {
-                        i18next.t("Unable to delete")
+                label = {
+                    <
+                    label htmlFor = "members-confirm" >
+                    <
+                    Trans >
+                    <
+                    strong > {
+                        `${membersCount}`
                     }
-                    content = {
-                        i18next.t(error)
+                    members < /strong> will be removed
+                    from the community. <
+                    /Trans> <
+                    /label>
+                }
+                checked = {
+                    checkboxMembers
+                }
+                onChange = {
+                    this.handleCheckboxChange
+                }
+                /> <
+                Checkbox
+                id = "records-confirm"
+                label = {
+                    <
+                    label htmlFor = "records-confirm" >
+                    <
+                    Trans >
+                    <
+                    strong > {
+                        `${recordsCount}`
                     }
-                    icon = "exclamation"
-                    className = "text-align-left"
-                    negative /
-                    >
-                )
-            } <
-            Button onClick = {
-                this.closeConfirmModal
-            }
-            disabled = {
-                loading
-            }
-            loading = {
-                loading
-            }
-            floated = "left" >
-            {
-                i18next.t("Cancel")
-            } <
-            /Button> <
-            Button negative onClick = {
-                () => this.handleDelete()
-            }
-            loading = {
-                loading
-            }
-            disabled = {
-                this.handleButtonDisabled(communitySlug) || loading
-            } >
-            {
-                i18next.t("Permanently delete")
-            } <
-            /Button> <
-            /Modal.Actions> <
-            /Modal> <
-            />
-        );
+                    records < /strong> will be removed
+                    from the community. <
+                    /Trans> <
+                    /label>
+                }
+                checked = {
+                    checkboxRecords
+                }
+                onChange = {
+                    this.handleCheckboxChange
+                }
+                /> <
+                Checkbox
+                id = "slug-confirm"
+                label = {
+                    <
+                    label htmlFor = "slug-confirm" >
+                    <
+                    Trans >
+                    You < strong > CANNOT < /strong> reuse the community identifier " {
+                        {
+                            communitySlug
+                        }
+                    }
+                    ". <
+                    /Trans> <
+                    /label>
+                }
+                checked = {
+                    checkboxSlug
+                }
+                onChange = {
+                    this.handleCheckboxChange
+                }
+                /> <
+                /Message.Content> <
+                /Message> <
+                /Modal.Content> <
+                Modal.Content >
+                    <
+                    Trans >
+                    Please type < strong > {
+                        {
+                            communitySlug
+                        }
+                    } < /strong> to confirm. <
+                    /Trans> <
+                    Input fluid value = {
+                        inputSlug
+                    }
+                onChange = {
+                    this.handleInputChange
+                }
+                /> <
+                /Modal.Content> <
+                Modal.Actions > {
+                        error && ( <
+                            ErrorMessage header = {
+                                i18next.t("Unable to delete")
+                            }
+                            content = {
+                                i18next.t(error)
+                            }
+                            icon = "exclamation"
+                            className = "text-align-left"
+                            negative /
+                            >
+                        )
+                    } <
+                    Button
+                onClick = {
+                    this.closeConfirmModal
+                }
+                disabled = {
+                    loading
+                }
+                loading = {
+                    loading
+                }
+                floated = "left" >
+                    {
+                        i18next.t("Cancel")
+                    } <
+                    /Button> <
+                    Button
+                negative
+                onClick = {
+                    () => this.handleDelete()
+                }
+                loading = {
+                    loading
+                }
+                disabled = {
+                        this.handleButtonDisabled(communitySlug) || loading
+                    } >
+                    {
+                        i18next.t("Permanently delete")
+                    } <
+                    /Button> <
+                    /Modal.Actions> <
+                    /Modal> <
+                    />
+            );
+        }
     }
-}
 
-DeleteCommunityModal.propTypes = {
-    onDelete: PropTypes.func.isRequired,
-    redirectURL: PropTypes.string.isRequired,
-    label: PropTypes.string.isRequired,
-    community: PropTypes.object.isRequired,
-};
+    DeleteCommunityModal.propTypes = {
+        onDelete: PropTypes.func.isRequired,
+        redirectURL: PropTypes.string.isRequired,
+        label: PropTypes.string.isRequired,
+        community: PropTypes.object.isRequired,
+    };
```

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot` & `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/cli.py` & `invenio-communities-7.0.0/invenio_communities/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,36 @@
 from invenio_search import current_search_client
 from invenio_search.engine import dsl
 from invenio_search.engine import search as search_engine
 from invenio_search.utils import build_alias_name
 
 from .fixtures.demo import create_fake_community
 from .fixtures.tasks import create_demo_community
-from .proxies import current_communities
+from .proxies import current_communities, current_identities_cache
 
 
 @click.group()
 def communities():
     """Invenio communities commands."""
 
 
+@click.group()
+def identity_cache():
+    """Invenio identity cache commands."""
+
+
+@identity_cache.command("clear")
+@with_appcontext
+def clear():
+    """Clears identity cache."""
+    click.secho("Clearing identity cache.", fg="green")
+    current_identities_cache.flush()
+    click.secho("Identity cache cleared.", fg="green")
+
+
 @communities.command("demo")
 @with_appcontext
 def demo():
     """Create 100 fake communities for demo purposes."""
     click.secho("Creating demo communities...", fg="green")
     faker = Faker()
     for _ in range(100):
```

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/__init__.py` & `invenio-communities-7.0.0/invenio_communities/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/dumpers/featured.py` & `invenio-communities-7.0.0/invenio_communities/communities/dumpers/featured.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/entity_resolvers.py` & `invenio-communities-7.0.0/invenio_communities/communities/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/api.py` & `invenio-communities-7.0.0/invenio_communities/communities/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json` & `invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/models.py` & `invenio-communities-7.0.0/invenio_communities/communities/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/systemfields/access.py` & `invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/access.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/records/systemfields/pidslug.py` & `invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/pidslug.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/resources/config.py` & `invenio-communities-7.0.0/invenio_communities/communities/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/resources/resource.py` & `invenio-communities-7.0.0/invenio_communities/communities/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/resources/serializer.py` & `invenio-communities-7.0.0/invenio_communities/communities/resources/serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/resources/ui_schema.py` & `invenio-communities-7.0.0/invenio_communities/communities/resources/ui_schema.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/schema.py` & `invenio-communities-7.0.0/invenio_communities/communities/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/__init__.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/components.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MetadataComponent,
     RelationsComponent,
     ServiceComponent,
 )
 from marshmallow.exceptions import ValidationError
 
 from ...proxies import current_roles
-from ...utils import on_membership_change
+from ...utils import on_user_membership_change
 from ..records.systemfields.access import VisibilityEnum
 
 
 class PIDComponent(ServiceComponent):
     """Service component for Community PIDs."""
 
     def set_slug(self, record, slug):
@@ -122,15 +122,15 @@
             system_identity,
             record.id,
             {"members": [member], "role": current_roles.owner_role.name},
             uow=self.uow,
         )
 
         # Invalidate the membership cache
-        on_membership_change(identity=identity)
+        on_user_membership_change(identity=identity)
 
 
 class FeaturedCommunityComponent(ServiceComponent):
     """Service component for featured community integration."""
 
     def featured_create(self, identity, data=None, record=None, **kwargs):
         """Featured create."""
```

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/config.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         "settings_html": CommunityLink("{+ui}/communities/{slug}/settings"),
         "logo": CommunityLink("{+api}/communities/{id}/logo"),
         "rename": CommunityLink("{+api}/communities/{id}/rename"),
         "members": CommunityLink("{+api}/communities/{id}/members"),
         "public_members": CommunityLink("{+api}/communities/{id}/members/public"),
         "invitations": CommunityLink("{+api}/communities/{id}/invitations"),
         "requests": CommunityLink("{+api}/communities/{id}/requests"),
+        "records": CommunityLink("{+api}/communities/{id}/records"),
     }
 
     action_link = CommunityLink(
         "{+api}/communities/{id}/{action_name}", when=can_perform_action
     )
 
     links_search = pagination_links("{+api}/communities{?args*}")
```

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/facets.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/links.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/links.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/results.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/service.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/service.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/sort.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/communities/services/uow.py` & `invenio-communities-7.0.0/invenio_communities/communities/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/config.py` & `invenio-communities-7.0.0/invenio_communities/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -291,7 +291,19 @@
     }]
 """
 
 # Preview: Feature flag for invenio-app-rdm v11
 COMMUNITIES_ADMINISTRATION_DISABLED = True
 
 COMMUNITIES_ALLOW_RESTRICTED = True
+
+# Cache duration
+# 60 seconds * 60 (1 hour) * 24 (1 day)
+COMMUNITIES_IDENTITIES_CACHE_TIME = 60 * 60 * 24
+
+# Redis URL Cache for identities
+COMMUNITIES_IDENTITIES_CACHE_REDIS_URL = "redis://localhost:6379/4"
+
+# Cache handler
+COMMUNITIES_IDENTITIES_CACHE_HANDLER = (
+    "invenio_communities.cache.redis:IdentityRedisCache"
+)
```

### Comparing `invenio-communities-6.7.0/invenio_communities/errors.py` & `invenio-communities-7.0.0/invenio_communities/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/ext.py` & `invenio-communities-7.0.0/invenio_communities/ext.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio communities extension."""
 
 from flask_principal import identity_loaded
+from invenio_accounts.signals import datastore_post_commit
+from invenio_base.utils import load_or_import_from_config
 from invenio_records_resources.services import FileService
 
 from invenio_communities.communities import (
     CommunityFileServiceConfig,
     CommunityResource,
     CommunityResourceConfig,
     CommunityService,
@@ -23,16 +25,17 @@
     MemberResource,
     MemberResourceConfig,
     MemberService,
     MemberServiceConfig,
 )
 
 from . import config
+from .cache.cache import IdentityCache
 from .roles import RoleRegistry
-from .utils import load_community_needs
+from .utils import load_community_needs, on_datastore_post_commit
 
 
 class InvenioCommunities(object):
     """Invenio extension."""
 
     def __init__(self, app=None):
         """Extension initialization."""
@@ -43,14 +46,15 @@
         """Flask application initialization."""
         self.init_config(app)
         app.extensions["invenio-communities"] = self
 
         self.init_services(app)
         self.init_resource(app)
         self.init_hooks(app)
+        self.init_cache(app)
 
     def init_config(self, app):
         """Initialize configuration.
 
         Override configuration variables with the values in this package.
         """
         for k in dir(config):
@@ -78,11 +82,25 @@
         self.members_resource = MemberResource(
             MemberResourceConfig,
             self.service.members,
         )
 
     def init_hooks(self, app):
         """Initialize hooks."""
+        datastore_post_commit.connect(on_datastore_post_commit)
 
         @identity_loaded.connect_via(app)
         def on_identity_loaded(_, identity):
             load_community_needs(identity)
+
+    def cache_handler(self, app):
+        """Return the cache handler."""
+        handler_func = load_or_import_from_config(
+            "COMMUNITIES_IDENTITIES_CACHE_HANDLER", app
+        )
+        handler = handler_func(app)
+        assert isinstance(handler, IdentityCache)
+        return handler
+
+    def init_cache(self, app):
+        """Initialize cache."""
+        self.cache = self.cache_handler(app)
```

### Comparing `invenio-communities-6.7.0/invenio_communities/fixtures/demo.py` & `invenio-communities-7.0.0/invenio_communities/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/fixtures/tasks.py` & `invenio-communities-7.0.0/invenio_communities/fixtures/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/generators.py` & `invenio-communities-7.0.0/invenio_communities/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/__init__.py` & `invenio-communities-7.0.0/invenio_communities/members/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/errors.py` & `invenio-communities-7.0.0/invenio_communities/members/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/api.py` & `invenio-communities-7.0.0/invenio_communities/members/records/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,14 +86,25 @@
             "request_id",
             "request",
             attrs=["status", "expires_at", "is_open"],
         ),
     )
 
     @classmethod
+    def get_memberships_from_group_ids(cls, identity, group_ids):
+        """Get community memberships for a given list of group ids."""
+        community_role_list = []
+        if group_ids:
+            query = cls.model_cls.query_memberships(
+                user_id=identity.id, group_ids=group_ids
+            )
+            community_role_list = [(str(comm_id), role) for comm_id, role in query]
+        return community_role_list
+
+    @classmethod
     def get_memberships(cls, identity):
         """Get community memberships for a given identity."""
         group_ids = []
         user = User.query.filter(User.id == identity.id).one_or_none()
         if user:
             group_ids = [r.id for r in user.roles]
 
@@ -110,36 +121,36 @@
         return cls(obj.data, model=obj)
 
     @classmethod
     def get_members(cls, community_id, members=None):
         """Get members of a community."""
         # Collect users and groups we are interested in
         user_ids = []
-        group_names = []
+        group_ids = []
         for m in members or []:
             if m["type"] == "group":
-                group_names.append(m["id"])
+                group_ids.append(m["id"])
             elif m["type"] == "user":
                 user_ids.append(m["id"])
             else:
                 raise InvalidMemberError(m)
 
         # Query
         q = cls.model_cls.query.filter(cls.model_cls.community_id == community_id)
 
         # Apply user and group query if applicable
         user_q = cls.model_cls.user_id.in_(user_ids)
         groups_q = cls.model_cls.group_id.in_(
-            db.session.query(Role.id).filter(Role.name.in_(group_names))
+            db.session.query(Role.id).filter(Role.id.in_(group_ids))
         )
-        if user_ids and group_names:
+        if user_ids and group_ids:
             q = q.filter(or_(user_q, groups_q))
         elif user_ids:
             q = q.filter(user_q)
-        elif group_names:
+        elif group_ids:
             q = q.filter(groups_q)
 
         return [cls(obj.data, model=obj) for obj in q.all()]
 
     @classmethod
     def has_members(cls, community_id, role=None):
         """Get members of a community."""
```

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json` & `invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/records/models.py` & `invenio-communities-7.0.0/invenio_communities/members/records/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             nullable=True,
         )
 
     @declared_attr
     def group_id(cls):
         """Foreign key to the related group."""
         return db.Column(
-            db.Integer(),
+            db.String(80),
             db.ForeignKey(Role.id, ondelete="RESTRICT"),
             nullable=True,
         )
 
     @declared_attr
     def request_id(cls):
         """Foreign key to the related request.
```

### Comparing `invenio-communities-6.7.0/invenio_communities/members/resources/config.py` & `invenio-communities-7.0.0/invenio_communities/members/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/resources/resource.py` & `invenio-communities-7.0.0/invenio_communities/members/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/components.py` & `invenio-communities-7.0.0/invenio_communities/members/services/components.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,60 +10,73 @@
 
 from flask_principal import Identity
 from invenio_accounts.models import Role
 from invenio_records_resources.services.records.components import ServiceComponent
 
 from invenio_communities.members.records.api import MemberMixin
 
-from ...utils import on_membership_change
+from ...proxies import current_identities_cache
+from ...utils import on_group_membership_change, on_user_membership_change
 
 
 class CommunityMemberCachingComponent(ServiceComponent):
     """Service component for community member caching."""
 
-    def _member_changed(self, member):
+    def _member_changed(self, member, community=None):
         """Call caching membership change function for user."""
-
-        def _get_user_ids_from_group_id(role_id):
-            r = Role.query.filter(Role.id == role_id).one()
-            return [u.id for u in r.users.all()]
-
         user_ids = []
         if isinstance(member, MemberMixin):
             if member.user_id:
                 user_ids = [member.user_id]
             elif member.group_id:
-                user_ids = _get_user_ids_from_group_id(member.group_id)
+                if not community:
+                    raise TypeError("Community must be defined.")
+                on_group_membership_change(str(community.id))
             else:
                 return
         elif isinstance(member, dict):
             if member.get("type") == "user":
                 user_ids = [member["id"]]
             elif member.get("type") == "group":
-                user_ids = _get_user_ids_from_group_id(member["id"])
+                if not community:
+                    raise TypeError("Community must be defined.")
+                on_group_membership_change(str(community.id))
             else:
                 return
         else:
             raise TypeError(
                 "Member must be 'MemberMixin' or 'dict' but was {type}".format(
                     type=type(member)
                 )
             )
 
         for user_id in user_ids:
-            on_membership_change(Identity(user_id))
+            on_user_membership_change(Identity(user_id))
 
     def accept_invite(self, identity, record=None, data=None, **kwargs):
         """On accept invite."""
         self._member_changed(record)
 
-    def members_add(self, identity, record=None, data=None, **kwargs):
+    def members_add(self, identity, record=None, community=None, data=None, **kwargs):
         """On member add (only for groups)."""
-        self._member_changed(record)
-
-    def members_delete(self, identity, record=None, data=None, **kwargs):
+        if record["type"] == "group":
+            role = Role.query.filter_by(id=record["id"]).one_or_none()
+            if role.is_managed:
+                users = role.users.all()
+                for user in users:
+                    on_user_membership_change(Identity(user.id))
+            else:
+                current_identities_cache.flush()
+        elif record["type"] == "user":
+            self._member_changed(record)
+
+    def members_delete(
+        self, identity, record=None, community=None, data=None, **kwargs
+    ):
         """On member delete."""
-        self._member_changed(record)
+        self._member_changed(record, community=community)
 
-    def members_update(self, identity, record=None, data=None, **kwargs):
+    def members_update(
+        self, identity, record=None, community=None, data=None, **kwargs
+    ):
         """On member update."""
-        self._member_changed(record)
+        self._member_changed(record, community=community)
```

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/config.py` & `invenio-communities-7.0.0/invenio_communities/members/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/facets.py` & `invenio-communities-7.0.0/invenio_communities/members/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/fields.py` & `invenio-communities-7.0.0/invenio_communities/members/services/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/request.py` & `invenio-communities-7.0.0/invenio_communities/members/services/request.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/schemas.py` & `invenio-communities-7.0.0/invenio_communities/members/services/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,16 @@
         current_identity = self.context["identity"]
         avatar = current_groups_service.links_item_tpl.expand(
             current_identity, fake_group_obj
         )["avatar"]
         return {
             "type": "group",
             "id": group["id"],
-            "name": group["id"] or "",
+            "name": group.get("name") or group["id"],
+            "description": group.get("description", ""),
             "avatar": avatar,
         }
 
 
 class MemberDumpSchema(PublicDumpSchema):
     """Schema for dumping members."""
```

### Comparing `invenio-communities-6.7.0/invenio_communities/members/services/service.py` & `invenio-communities-7.0.0/invenio_communities/members/services/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,15 @@
 
             factory(identity, community, role, visible, m, message, uow)
             # Run components
             self.run_components(
                 action,
                 identity,
                 record=m,
+                community=community,
                 errors=None,
                 uow=uow,
             )
 
         return True
 
     def _add_factory(
@@ -237,23 +238,14 @@
         member,
         message,
         uow,
         active=True,
         request_id=None,
     ):
         """Add a member to the community."""
-        # TODO: inefficient to do here, should be done in bulk instead.
-        if member["type"] == "group":
-            try:
-                # member['id'] is mapped from role.name
-                # (check invenio-users-resources)
-                member["id"] = Role.query.filter_by(name=member["id"]).one().id
-            except NoResultFound as e:
-                raise InvalidMemberError(member) from e
-
         member_arg = {member["type"] + "_id": member["id"]}
         try:
             # Integrity checks happens here which will validate:
             # - if a user/group is already a member
             # - if a user is already invited
             member = self.record_cls.create(
                 {},
@@ -592,14 +584,15 @@
             member.visible = visible
 
         # Run components
         self.run_components(
             "members_update",
             identity,
             record=member,
+            community=community,
             errors=None,
             uow=uow,
         )
 
         uow.register(RecordCommitOp(member, self.indexer))
 
         return True
@@ -635,14 +628,15 @@
                 member=m,
             )
             # Run components
             self.run_components(
                 "members_delete",
                 identity,
                 record=m,
+                community=community,
                 errors=None,
                 uow=uow,
             )
             uow.register(RecordDeleteOp(m, self.indexer, force=True))
 
         # Make sure we're not left owner-less
         if not self.record_cls.has_members(
```

### Comparing `invenio-communities-6.7.0/invenio_communities/notifications/generators.py` & `invenio-communities-7.0.0/invenio_communities/notifications/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/permissions.py` & `invenio-communities-7.0.0/invenio_communities/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/records/records/models.py` & `invenio-communities-7.0.0/invenio_communities/records/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/context.py` & `invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/context.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/field.py` & `invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/field.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/records/records/systemfields/communities/manager.py` & `invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/roles.py` & `invenio-communities-7.0.0/invenio_communities/roles.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/searchapp.py` & `invenio-communities-7.0.0/invenio_communities/searchapp.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html` & `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/af/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/da/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/de/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/el/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/en/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/es/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/et/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/it/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/messages.pot` & `invenio-communities-7.0.0/invenio_communities/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/no/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/views/__init__.py` & `invenio-communities-7.0.0/invenio_communities/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/views/api.py` & `invenio-communities-7.0.0/invenio_communities/views/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/views/communities.py` & `invenio-communities-7.0.0/invenio_communities/views/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/views/decorators.py` & `invenio-communities-7.0.0/invenio_communities/views/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/views/ui.py` & `invenio-communities-7.0.0/invenio_communities/views/ui.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities/webpack.py` & `invenio-communities-7.0.0/invenio_communities/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/invenio_communities.egg-info/PKG-INFO` & `invenio-communities-7.0.0/invenio_communities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-communities
-Version: 6.7.0
+Version: 7.0.0
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-communities
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,22 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 7.0.0 (released 2023-06-15)
+        -----------------------------------
+        
+        - cache: adds unmanaged groups to be cached and loaded in the identity
+        - adds identity cache
+        - add groups as community members
+        - assets: display metrics on deletion modal
+        
         Version 6.7.0 (released 2023-06-07)
         -----------------------------------
         
         - notifications: add member recipient generator
         - tests: add notification member recipient generator test case
         - services: add extra_filter param
         - services: provide explicit scan params
```

### Comparing `invenio-communities-6.7.0/invenio_communities.egg-info/SOURCES.txt` & `invenio-communities-7.0.0/invenio_communities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,28 @@
 invenio_communities/errors.py
 invenio_communities/ext.py
 invenio_communities/generators.py
 invenio_communities/permissions.py
 invenio_communities/proxies.py
 invenio_communities/roles.py
 invenio_communities/searchapp.py
+invenio_communities/tasks.py
 invenio_communities/utils.py
 invenio_communities/webpack.py
 invenio_communities.egg-info/PKG-INFO
 invenio_communities.egg-info/SOURCES.txt
 invenio_communities.egg-info/dependency_links.txt
 invenio_communities.egg-info/entry_points.txt
 invenio_communities.egg-info/not-zip-safe
 invenio_communities.egg-info/requires.txt
 invenio_communities.egg-info/top_level.txt
 invenio_communities/administration/__init__.py
 invenio_communities/administration/communities.py
+invenio_communities/alembic/02cd82910727_update_role_id_type_upgrade.py
+invenio_communities/alembic/37b21951084c_update_role_id_type_downgrade.py
 invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
 invenio_communities/alembic/90642d415317_create_communities_branch.py
 invenio_communities/alembic/__init__.py
 invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
 invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
 invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
 invenio_communities/alembic/fbe746957cfc_create_member_tables.py
@@ -234,14 +237,17 @@
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
 invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
+invenio_communities/cache/__init__.py
+invenio_communities/cache/cache.py
+invenio_communities/cache/redis.py
 invenio_communities/communities/__init__.py
 invenio_communities/communities/entity_resolvers.py
 invenio_communities/communities/schema.py
 invenio_communities/communities/dumpers/featured.py
 invenio_communities/communities/records/__init__.py
 invenio_communities/communities/records/api.py
 invenio_communities/communities/records/models.py
@@ -406,14 +412,15 @@
 invenio_communities/views/__init__.py
 invenio_communities/views/api.py
 invenio_communities/views/communities.py
 invenio_communities/views/decorators.py
 invenio_communities/views/ui.py
 tests/conftest.py
 tests/test_notifications.py
+tests/cache/test_identity_redis_cache.py
 tests/communities/conftest.py
 tests/communities/test_alembic.py
 tests/communities/test_cli.py
 tests/communities/test_community_ui_serializer.py
 tests/communities/test_components.py
 tests/communities/test_relations_organizations.py
 tests/communities/test_relations_types.py
```

### Comparing `invenio-communities-6.7.0/invenio_communities.egg-info/entry_points.txt` & `invenio-communities-7.0.0/invenio_communities.egg-info/entry_points.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [flask.commands]
 communities = invenio_communities.cli:communities
+identity-cache = invenio_communities.cli:identity_cache
 
 [invenio_administration.views]
 invenio_communities_details = invenio_communities.administration.communities:CommunityDetailView
 invenio_communities_list = invenio_communities.administration.communities:CommunityListView
 
 [invenio_assets.webpack]
 invenio_communities = invenio_communities.webpack:communities
@@ -20,15 +21,16 @@
 invenio_communities = invenio_communities:InvenioCommunities
 
 [invenio_base.blueprints]
 invenio_communities = invenio_communities.views:create_ui_blueprint
 invenio_communities_ext = invenio_communities.views:blueprint
 
 [invenio_celery.tasks]
-invenio_communities = invenio_communities.fixtures.tasks
+invenio_communities = invenio_communities.tasks
+invenio_communities_fixtures = invenio_communities.fixtures.tasks
 
 [invenio_db.alembic]
 invenio_communities = invenio_communities:alembic
 
 [invenio_db.models]
 invenio_communities = invenio_communities.communities.records.models
 invenio_communities_members = invenio_communities.members.records.models
```

### Comparing `invenio-communities-6.7.0/run-js-linter.sh` & `invenio-communities-7.0.0/run-js-linter.sh`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/run-tests.sh` & `invenio-communities-7.0.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/setup.cfg` & `invenio-communities-7.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,27 @@
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0
 	Faker>=2.0.3
 	invenio-app>=1.3.4,<2.0.0
 	invenio-db[postgresql,mysql]>=1.0.14,<2.0.0
-	pytest-invenio>=2.1.0,<3.0.0
+	pytest-invenio>=2.1.4,<3.0.0
 	sphinx>=4.5.0
 elasticsearch7 = 
 	invenio-search[elasticsearch7]>=2.1.0,<3.0.0
 opensearch1 = 
 	invenio-search[opensearch1]>=2.1.0,<3.0.0
 opensearch2 = 
 	invenio-search[opensearch2]>=2.1.0,<3.0.0
 
 [options.entry_points]
 flask.commands = 
 	communities = invenio_communities.cli:communities
+	identity-cache = invenio_communities.cli:identity_cache
 invenio_base.apps = 
 	invenio_communities = invenio_communities:InvenioCommunities
 invenio_base.api_apps = 
 	invenio_communities = invenio_communities:InvenioCommunities
 invenio_base.blueprints = 
 	invenio_communities_ext = invenio_communities.views:blueprint
 	invenio_communities = invenio_communities.views:create_ui_blueprint
@@ -62,15 +63,16 @@
 	communities = invenio_communities.communities.records.mappings
 	communitymembers = invenio_communities.members.records.mappings
 invenio_jsonschemas.schemas = 
 	communities = invenio_communities.communities.records.jsonschemas
 invenio_assets.webpack = 
 	invenio_communities = invenio_communities.webpack:communities
 invenio_celery.tasks = 
-	invenio_communities = invenio_communities.fixtures.tasks
+	invenio_communities_fixtures = invenio_communities.fixtures.tasks
+	invenio_communities = invenio_communities.tasks
 invenio_requests.entity_resolvers = 
 	communities = invenio_communities.communities.entity_resolvers:CommunityResolver
 invenio_requests.types = 
 	community_invitation = invenio_communities.members.services.request:CommunityInvitation
 invenio_i18n.translations = 
 	messages = invenio_communities
 invenio_administration.views =
```

### Comparing `invenio-communities-6.7.0/tests/communities/conftest.py` & `invenio-communities-7.0.0/tests/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_alembic.py` & `invenio-communities-7.0.0/tests/communities/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_cli.py` & `invenio-communities-7.0.0/tests/communities/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_community_ui_serializer.py` & `invenio-communities-7.0.0/tests/communities/test_community_ui_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_components.py` & `invenio-communities-7.0.0/tests/communities/test_components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_relations_organizations.py` & `invenio-communities-7.0.0/tests/communities/test_relations_organizations.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_relations_types.py` & `invenio-communities-7.0.0/tests/communities/test_relations_types.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_resources.py` & `invenio-communities-7.0.0/tests/communities/test_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/test_services.py` & `invenio-communities-7.0.0/tests/communities/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/communities/tests_views.py` & `invenio-communities-7.0.0/tests/communities/tests_views.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/conftest.py` & `invenio-communities-7.0.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,23 @@
     # Define files storage class list
     app_config["FILES_REST_STORAGE_CLASS_LIST"] = {
         "L": "Local",
         "F": "Fetch",
         "R": "Remote",
     }
     app_config["FILES_REST_DEFAULT_STORAGE_CLASS"] = "L"
+    app_config["COMMUNITIES_IDENTITIES_CACHE_TIME"] = 2
+
+    # Redis URL Cache for identities
+    app_config["COMMUNITIES_IDENTITIES_CACHE_REDIS_URL"] = "redis://localhost:6379/4"
+
+    # Cache handler
+    app_config[
+        "COMMUNITIES_IDENTITIES_CACHE_HANDLER"
+    ] = "invenio_communities.cache.redis:IdentityRedisCache"
 
     return app_config
 
 
 @pytest.fixture(scope="module")
 def create_app(instance_path):
     """Application factory fixture."""
@@ -138,15 +147,15 @@
     database.session.commit()
     return users
 
 
 @pytest.fixture(scope="module")
 def group(database):
     """Group."""
-    r = Role(name="it-dep")
+    r = Role(id="it-dep", name="it-dep")
     database.session.add(r)
     database.session.commit()
     return r
 
 
 @pytest.fixture(scope="module")
 def owner(users):
@@ -199,15 +208,15 @@
     """Store 1 role with 'superuser-access' ActionNeed.
 
     WHY: This is needed because expansion of ActionNeed is
          done on the basis of a User/Role being associated with that Need.
          If no User/Role is associated with that Need (in the DB), the
          permission is expanded to an empty list.
     """
-    role = Role(name="admin-access")
+    role = Role(id="admin-access", name="admin-access")
     db.session.add(role)
 
     action_role = ActionRoles.create(action=action_admin_access, role=role)
     db.session.add(action_role)
 
     db.session.commit()
 
@@ -219,15 +228,15 @@
     """Store 1 role with 'superuser-access' ActionNeed.
 
     WHY: This is needed because expansion of ActionNeed is
          done on the basis of a User/Role being associated with that Need.
          If no User/Role is associated with that Need (in the DB), the
          permission is expanded to an empty list.
     """
-    role = Role(name="superuser-access")
+    role = Role(id="superuser-access", name="superuser-access")
     db.session.add(role)
 
     action_role = ActionRoles.create(action=superuser_access, role=role)
     db.session.add(action_role)
 
     db.session.commit()
```

### Comparing `invenio-communities-6.7.0/tests/members/conftest.py` & `invenio-communities-7.0.0/tests/members/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/members/test_members_components.py` & `invenio-communities-7.0.0/tests/members/test_members_components.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,173 +4,173 @@
 #
 # Invenio-Communities is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Test components."""
 
 from invenio_access.permissions import system_identity
-from invenio_cache import current_cache
 
+from invenio_communities.proxies import current_identities_cache
 from invenio_communities.utils import identity_cache_key
 
 
 def test_accept_invite_cache_clear(
     requests_service, invite_request_id, invite_user, db, search_clear
 ):
     """Test that the community member cached entries are cleared."""
-    current_cache.clear()
+    current_identities_cache.flush()
     cache_key = identity_cache_key(invite_user.identity)
 
     invite_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
 
     # cached entry should be cleared on accept_invite
     requests_service.execute_action(invite_user.identity, invite_request_id, "accept")
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     invite_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
 
 def test_member_delete_cache_clear(
     member_service, community, new_user, db, search_clear
 ):
     """Test that the community member cached entries are cleared."""
-    current_cache.clear()
+    current_identities_cache.flush()
     cache_key = identity_cache_key(new_user.identity)
 
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
 
     # cached entry should be cleared on add
     add_data = {
         "members": [{"type": "user", "id": str(new_user.id)}],
         "role": "reader",
     }
     member_service.add(system_identity, community._record.id, add_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
     # cached entry should be cleared on delete
     delete_data = {
         "members": [{"type": "user", "id": str(new_user.id)}],
     }
     member_service.delete(system_identity, community._record.id, delete_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
 
 
 def test_member_add_cache_clear(member_service, community, new_user, db, search_clear):
     """Test that the community member cached entries are cleared."""
-    current_cache.clear()
+    current_identities_cache.flush()
     cache_key = identity_cache_key(new_user.identity)
 
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
 
     # cached entry should be cleared on add
     add_data = {
         "members": [{"type": "user", "id": str(new_user.id)}],
         "role": "reader",
     }
     member_service.add(system_identity, community._record.id, add_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
 
 def test_member_update_cache_clear(
     member_service, community, new_user, db, search_clear
 ):
     """Test that the community member cached entries are cleared."""
-    current_cache.clear()
+    current_identities_cache.flush()
     cache_key = identity_cache_key(new_user.identity)
 
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
 
     # cached entry should be cleared on add
     add_data = {
         "members": [{"type": "user", "id": str(new_user.id)}],
         "role": "reader",
     }
     member_service.add(system_identity, community._record.id, add_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
     update_data = {
         "members": [{"type": "user", "id": str(new_user.id)}],
         "role": "reader",
     }
     member_service.update(system_identity, community._record.id, update_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     new_user.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
 
 def test_group_actions_cache_clear(
     member_service, restricted_community, admin, db, search_clear
 ):
     """Test that the community member cached entries are cleared on group actions."""
-    current_cache.clear()
+    current_identities_cache.flush()
     cache_key = identity_cache_key(admin.identity)
 
     admin.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
 
     # cached entry should be cleared for group members on add
     data = {
         "members": [{"type": "group", "id": "admin-access"}],
         "role": "reader",
     }
 
     # cached entry should be cleared for group members
     member_service.add(system_identity, restricted_community._record.id, data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
 
     admin.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
     # cached entry should be cleared for group members on update
     update_data = {
         "members": [{"type": "group", "id": "admin-access"}],
         "role": "manager",
     }
     member_service.update(system_identity, restricted_community._record.id, update_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
 
     admin.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 1
 
     # cached entry should be cleared for group members on delete
     delete_data = {
         "members": [{"type": "group", "id": "admin-access"}],
     }
     member_service.delete(system_identity, restricted_community._record.id, delete_data)
-    community_roles = current_cache.get(cache_key)
-    assert community_roles == None
+    community_roles = current_identities_cache.get(cache_key)
+    assert community_roles is None
     admin.refresh()
-    community_roles = current_cache.get(cache_key)
+    community_roles = current_identities_cache.get(cache_key)
     assert len(community_roles) == 0
```

### Comparing `invenio-communities-6.7.0/tests/members/test_members_no_groups.py` & `invenio-communities-7.0.0/tests/members/test_members_no_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/members/test_members_resource.py` & `invenio-communities-7.0.0/tests/members/test_members_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/members/test_members_services.py` & `invenio-communities-7.0.0/tests/members/test_members_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from invenio_cache import current_cache
 from invenio_records_resources.services.errors import PermissionDeniedError
 from invenio_requests.records.api import RequestEvent
 from marshmallow import ValidationError
 
 from invenio_communities.members.errors import AlreadyMemberError, InvalidMemberError
 from invenio_communities.members.records.api import ArchivedInvitation, Member
+from invenio_communities.proxies import current_identities_cache
 
 
 #
 # Add members
 #
 @pytest.mark.parametrize(
     "actor,role",
@@ -123,17 +124,17 @@
     )
     member_service.add(system_identity, community._record.id, data)
 
 
 def test_add_invalid_data(member_service, community, owner, group, db):
     """Test various forms of invalid data."""
     # Invalid group id
-    data = {"members": [{"type": "group", "id": "invalid"}], "role": "reader"}
+    data = {"members": [{"type": "group", "id": 123}], "role": "reader"}
     assert pytest.raises(
-        InvalidMemberError,
+        ValidationError,
         member_service.add,
         owner.identity,
         community._record.id,
         data,
     )
     # Missing member id
     data = {"members": [{"type": "group"}], "role": "reader"}
@@ -600,15 +601,15 @@
     )
 
 
 def test_leave_denied(db, member_service, community, any_user, invite_user):
     """No permission for others"""
     # some test is not undoing membership correctly
     # FIXME when https://github.com/inveniosoftware/pytest-invenio/issues/30
-    current_cache.clear()
+    current_identities_cache.flush()
     any_user.refresh()
     data = {"members": [{"type": "user", "id": str(any_user.id)}]}
     pytest.raises(
         PermissionDeniedError,
         member_service.delete,
         any_user.identity,
         community._record.id,
```

### Comparing `invenio-communities-6.7.0/tests/records/conftest.py` & `invenio-communities-7.0.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/records/mock_module/api.py` & `invenio-communities-7.0.0/tests/records/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/records/mock_module/models.py` & `invenio-communities-7.0.0/tests/records/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/records/test_mockrecords_api.py` & `invenio-communities-7.0.0/tests/records/test_mockrecords_api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.7.0/tests/test_notifications.py` & `invenio-communities-7.0.0/tests/test_notifications.py`

 * *Files identical despite different names*

