CHANGELOG for Sulu CMF
======================

* dev-develop
    * BUGFIX      #474  [SULU-STANDARD]  Registered SuluGeneratorBundle

* 1.0.10 (2015-09-14)
    * HOTFIX      #1572 [ContentBundle]         Fixed select overlay for internal link node type
    * HOTFIX      #1567 [Document]              Fixed localized property for url property
    * HOTFIX      #1568 [ContentBundle]         Fixed copy extension data
    * HOTFIX      #1577 [DocumentManagerBundle] Made caching directory for DocumentManager configureable

* 1.0.9 (2015-08-31)
    * HOTFIX      #1539 [WebsiteBundle]  Fixed canonical tag for shadow pages
    * HOTFIX      #1537 [WebsiteBundle]  Fixed format of hreflang-tag locale
    * HOTFIX      #1532 [WebsiteBundle]  Fixed redirect to external pages
    * HOTFIX      #1511 [ContentBundle]  Fixed single-internal-link overlay URL
    * HOTFIX      #1521 [MediaBundle]    Fixed media-selection events for preview update

* 1.0.8 (2015-08-18)
    * HOTFIX      #---- [Sulu-Standard]  Updated dependencies because of bug in jackalope-jackrabbit

* 1.0.7 (2015-08-11)
    * HOTFIX      #1469 [ContentBundle]  fixed displayOptions in media selection
    * HOTFIX      #1468 [SnippetBundle]  Fixed default language for snippets in administration
>>>>>>> master

* 1.0.6 (2015-08-05)
    * HOTFIX      #1448 [AdminBundle]    Fixed additional system languages

* 1.0.5 (2015-08-03)
    * HOTFIX      #--   [AdminBundle]    Fixed ckeditor overlay buttons for windows

* 1.0.4 (2015-07-28)
    * HOTFIX      #1427 [ContentBundle]  Added external link migration
    * HOTFIX      #1419 [ContentBundle]  Fixed tags, categories and navigation context for shadow pages

* 1.0.3 (2015-07-23)
    * HOTFIX      #1394 [MediaBundle]    Added regex replace for media download to avoid umlauts error
    * HOTFIX      #1391 [All]            Removed partial load hints
    * HOTFIX      #1393 [SnippetBundle]  Added try-catch to avoid exception for snippet load
    * HOTFIX      #1395 [ContentBundle]  Fixed cache-lifetime is required bug for lifetime "0"
    * HOTFIX      #1386 [ContentBundle]  Fixed hard-coded values in search metadata
    * HOTFIX      #1400 [SnippetBundle]  Fixed block sorting in snippet form
    * HOTFIX      #1378 [ContentBundle]  Fixed sorting of pages
    * HOTFIX      #1414 [ContentBundle]  Set published property in resolved smart content to date instead boolean

* 1.0.2 (2015-07-13)
    * HOTFIX      #479  [SULU-STANDARD]  Use sulu:build for setting up test database
    * HOTFIX      #1355 [CoreBundle]     Fixed creator id for website document
    * HOTFIX      #1346 [ContentBundle]  Reversed order of paths to enable overriding of templates again
    * HOTFIX      #1366 [CoreBundle]     Fixed build command for not existing database

* 1.0.1 (2015-07-06)
    * HOTFIX      #475  [All]            Fixed inheritance of configs and moved liip-theme config
    * HOTFIX      #1338 [Content]        Fixed wrong check for block type meta title

* 1.0.0 (2015-07-01)
    * ENHANCEMENT #471  [SULU-STANDARD]  Cleanup config to reduce merge conflicts
    * ENHANCEMENT #1319 [ContentBundle]  Fixed location of cached structures
    * BUGFIX      #1316 [ContentBundle]  Reenabled csrf protection and disabled it only for the content mapper
    * FEATURE     #1314 [SecurityBundle] Enable new persistence handling for User & Role.
    * FEATURE     #1314 [AdminBundle]    Added search component to the sulu dashboard
    * BUGFIX      #1313 [MediaBundle]    Fixed image conversion in environments where open_basedir is enabled
    * BUGFIX      #1308 [ContactBundle]  Fixed adding a new contact-account relation in contacts tab of account
    * ENHANCEMENT #1302 [MediaBundle]    Removed 'partial-load' hint from getMediaById repository function.
    * BUGFIX      #1172 [ContentBundle]  Fix hreflang meta tags, remove invalid title meta tag
    * BUGFIX      #1172 [ContentBundle]  Fixed ckeditor in blocks for IE11
    * ENHANCEMENT #1040 [ContentBundle]  Added validation for required tag name
    * FEATURE     #1278 [ContentBundle]  Implemented webspace structure provider
    * FEATURE     #1273 [SnippetBundle]  Removed snippet state from ui and set default published
    * FEATURE     #1281 [ContentBundle]  Added default-template config to webspace theme
    * FEATURE     #1315 [ContentBundle]  Fixed translator locale for preview
    * BUGFIX      #1023 [ContactBundle]  Fixed back to list in contact-list

* 1.0.0-RC3 (2015-06-24)
    * HOTFIX      #1306 [ContentBundle]  Fixed migration commands for jackrabbit
    * ENHANCEMENT #1260 [All]            Removed or renamed all old update commands
    * ENHANCEMENT #1090 [All]            Introduced DocumentManager
    * BUGFIX      #1295 [ContentBundle]  Fixed call of changed event from MassiveSearchBundle
    * ENHANCEMENT #1230 [ContactBundle]  Introduced the new `PersistenceBundle` which makes entities easy replaceable. 
                                         Added this functionality for the contact entity.

* 1.0.0-RC2 (2015-06-17)
    * BUGFIX      #1264 [ContentBundle]  fixed save of changed block type
    * BUGFIX      #1259 [ContentBundle]  Fixed internal link assignment delete
    * BUGFIX      #1244 [WebsiteBundle]  Updated LiipThemeBundle to get assetic bugfix
    * BUGFIX      #1254 [SnippetBundle]  Fixed snippet assigment delete
    * BUGFIX      #1250 [ContactBundle]  Fixed document assigment delete in contact area
    * ENHANCEMENT #1251 [SecurityBundle] Refactored PasswordResetting controller for better reusability
    * BUGFIX      #1253 [MediaBundle]    Improved speed for media list query
    * BUGFIX      #1245 [ContentBundle]  Ensure that concrete languages will be serialized as array not as object
    * FEATURE     #1248 [ContentBundle]  Added cleanup resource-locator history command
    * BUGFIX      #1243 [ContentBundle]  Added ignore of ghost pages when content copy locale
    * ENHANCEMENT #1234 [All]            Prefix twig extension functions with "sulu_"
    * ENHANCEMENT #1237 [AdminBundle]    Fixed typos in behat tests
    * BUGFIX      #1235 [ContentBundle]  Fixed delete page which has children with history url
    * BUGFIX      #1231 [ContentBundle]  Fixed wrong behaviour if you edit a shadow page
    * BUGFIX      #1216 [SecurityBundle] Moved settings action to non-secured ProfileController
    * BUGFIX      #1213 [ContentBundle]  Fixed redirect of external links
    * FEATURE     #1214 [MediaBundle]    Added language chooser in "all media" view and in edit-media overlay
    * BUGFIX      #1211 [WebsiteBundle]  Fixed merge of test-page childs into upper layer in website navigation
    * ENHANCMENT  #1206 [SecurityBundle] Corrected translation for roles entry in navigation
    * BUGFIX      #1203 [AdminBundle]    Fixed routes for tabs
    * BUGFIX      #1199 [ContentBundle]  URL of shadow pages are not delivered in the urls array
    * BUGFIX      #1207 [ContentBundle]  Added additional query before generate new url
    * BUGFIX      #1169 [AdminBundle]    Fixed sidebar issue (prepending div instead of appending)
    * ENHANCEMENT #1159 [SecurityBundle] Change role naming to keep symfony2 conventions.
    * BUGFIX      #1156 [MediaBundle]    Fix mimetype check for ghostscript
    * BUGFIX      #1163 [ContentBundle]  Set existing default for content language
    
* 1.0.0-RC1 (2015-05-29)
    * ENHANCEMENT #1148 [SecurityBundle] Moved user specific code from UserController to UserManager
    * BUGFIX      #1147 [MediaBUndle]    Fixes fileVersion created date
    * ENHANCEMENT #1134 [MediaBundle]    Add parameter to view pdf in browser instead of downloading it immediately
    * ENHANCEMENT #1055 [MediaBundle]    Use tagged services instead of prefix for image converter commands
    * ENHANCEMENT #1144 [CacheBundle]    Changed dependencies from guzzle and HTTPCacheBundle
    * BUGFIX      #1141 [WebsiteBundle]  Added smaller version of logo and fixed twig syntax errors for profiler
    * BUGFIX      #1075 [WebsiteBundle]  Fixed sitemap add validation for requested domain
    * BUGFIX      #1124 [ContentBundle]  Fixed preview with multiple blocks
    * BUGFIX      #1123 [ContentBundle]  Fixed block behaviour on template change
    * ENHANCEMENT #1118 [SecurityBundle] Add possibility to enable SecurityChecker and SuluSecurityListener via configuration
    * ENHANCEMENT #1113 [ContactBundle]  Added sorting by last-name in accounts-contact tab
    * ENHANCEMENT #1100 [ContentBundle]  Replaced the checkboxes with radio buttons in overlay for creating node in new localization
    * ENHANCEMENT #1088 [ContactBundle]  Moved initialization of field-descriptors before init of list-builder in
                                         accounts cget action
    * ENHANCEMENT #1053 [Util]           Remove unused UuidUtils class
    * ENHANCEMENT #1038 [MediaBundle]    Added counter for selected images; Disabled drag event for links and
                                         images inside the overlay; Store media assignement display options in user settings
    * BUGFIX      #1051 [Website]        Throw NoValidWebspaceException if no valid webspaces are found
    * BUGFIX      #1089 [Media/Search]   Do not set image URL for non-images in the search results
    * BUGFIX      #996  [ContentBundle]  Fixed change language in add form
    * BUGFIX      #725  [Webspace]       Fixed trailing slash in defining url in webspace config

* 0.18.2 (2015-05-18)
    * HOTFIX      #1094 [MediaBundle]    Fixed media overlay version tab appearance

* 0.18.1 (2015-05-09)
    * HOTFIX      #1079 [SearchBundle]   Fix webspace-key index for content pages

* 0.18.0 (2015-05-08)
    * ENHANCEMENT #797  [SearchBundle]   Rebuild command removed, now hooks into massive:search:index:rebuild
    * ENHANCEMENT #797  [SearchBundle]   Unpublished pages are no longer deindexed - a "state" field has been added, see UPGRADE.md
    * ENHANCEMENT #797  [ContactBundle]  Contacts and Accounts have massive search mappings
    * ENHANCEMENT #1076 [AdminBundle]    Moved some translations from admin-bundle to their specific bundles
    * ENHANCEMENT #1057 [All]            Upgrade of jackalope 1.2
    * BUGFIX      #1072 [ContentBundle]  Cropping of long rlps in history overlay
    * BUGFIX      #1067 [SecurityBundle] Increase locale db field for big locale jsons
    * BUGFIX      #1065 [AdminBundle]    Second try: Fixed 1Password css bug on login screen
    * BUGFIX      #--   [AdminBundle]    Fixed login for IE see [commit](https://github.com/sulu-io/sulu/commit/a50e48aa83d360b93b5db0a63300c2799d3bc8ab)
    * BUGFIX      #1045 [MediaBundle]    Fixed upload new media version
    * FEATURE     #496  [ContentBundle]  SmartContent: change default tag filter to OR operation and user can decide to use OR or AND    
    * ENHANCEMENT #1039 [ContactBundle]  Auto select new title or positions in contact form
    * ENHANCEMENT #--   [MediaBundle]    Added function to get base media types
    * ENHANCEMENT #1031 [MediaBundle]    Fixed success label for collection delete
    * FEATURE     #977  [MediaBundle]    Made Format Cache parameters configurable, prefix ghostscript path parameter with sulu_media.
    * BUGFIX      #945  [WebsiteBundle]  Fix Redirect url with query string correctly and trailing slash
    * ENHANCEMENT #1029 [All]            Removed prefixes from content navigation providers and admins
    * FEATURE     #1014 [MediaBundle]    Added media preview in edit overlay
    * BUGFIX      #1026 [MediaBundle]    Fixed collection and category behat tests 
    * BUGFIX      #1030 [WebsiteBundle]  Fixed exception-controller to resolve parameters like website-controller
    * FEATURE     #1030 [WebsiteBundle]  Added configuration for error templates to webspace-config

* 0.17.0 (2015-04-20)
    * ENHANCEMENT #437 [MediaBundle]     Delete response_headers and ghostscript path from config, working defaults added 
    * FEATURE     #931 [MediaBundle]     Add Media Version History Tab
    * ENHANCEMENT #428 [sulu-standard]   Removed ladybug bundle
    * FEATURE     #919 [ContentBundle]   Add Text editor option enable iframe, script tag and delete godMode
    * FEATURE     #203 [sulu-standard]   Text editor configurable height, maxHeight for autogrow
    * BUGFIX      #186 [sulu-standard]   Freeze Browser in Source Edit mode change (CKEditor Update)
    * BUGFIX      #411 [sulu-standard]   Table Right Click Menu (CKEditor Update)
    * FEATURE     #419 [sulu-standard]   Added maintenance mode, which can be enabled by setting environment variable
                                         SULU_MAINTENANCE true
    * FEATURE     #838 [SecurityBundle]  AJAX-Login and resetting of password
    * FEATURE     #838 [AdminBundle]     Login UI
    * BUGFIX      #1020 [ContactBundle]  Fixed organization go back type bug
    * BUGFIX      #1021 [SecurityBundle] Only check security for not-null security contexts
    * BUGFIX      #1009 [MediaBundle]    Fix media download url
    * ENHANCEMENT #1005 [ContactBundle]  Added security checks for contacts and accounts
    * BUGFIX      #1008 [AdminBundle]    Fixed 1Password css bug on login screen
    * BUGFIX      #1004 [MediaBundle]    Fix animated gifs
    * BUGFIX      #1002 [ContentBundle]  Changed internal link title for navigation, smartcontent and internal link
    * FEATURE     #935 [MediaBundle]     Added new media selection
    * BUGFIX      #952 [MediaBundle]     Fix coffee icon fallback in media thumbnail view
    * ENHANCEMENT #951 [MediaBundle]     Made path to image-formats.xml configurateable
    * BUGFIX      #968 [MediaBundle]     Add wildcard support for media type check
    * ENHANCEMENT #988 [ContentBundle]   Set locale on render request
    * BUGFIX      #994 [CategoryBundle]  Fixed category search  
    * ENHANCEMENT #988 [MediaBundle]     Set working defaults for ghostscript and caching headers
    * BUGFIX      #976 [MediaBundle]     Fix media scale mode parameter
    * FEATURE     #975 [MediaBundle]     Make Storage path and segments configurateable
    * BUGFIX      #973 [All]             Added handling of anonymous user token
    * BUGFIX      #970 [SecurityBundle]  Fixed select all bug in permissions tab
    * FEATURE     #941 [SecurityBundle]  Adding permissions on an object basis
    * FEATURE     #931 [MediaBundle]     Version History Tab
    * FEATURE     #923 [ContactBundle]   Extract CRM to own Bundles
    * BUGFIX      #922 [ContentBundle]   Fixed URL Generation after copying language of a child node
    * FEATURE     #732 [All]             Automatic mapping and assignation of changer, creator, changed and changer.
    * FEATURE     #891 [All]             Added (css) class property to field descriptors, updated husky and fixed an issue when merging settings with matchings
    * FEATURE     #884 [MediaBundle]     Loaders on media delete and media edit
    * BUGFIX      #884 [AdminBundle]     Fix for login displacement issues
    * BUGFIX      #884 [MediaBundle]     Fix for uploading bug on click on dropzone
    * ENHANCEMENT #877 [SecurityBundle]  Extracted some classes to component
    * BUGFIX      #863 [AdminBundle]     Fix for issue that navigation moved content on uncollapse
    * BUGFIX      #863 [MediaBundle]     Fix for not working image upload with click on the dropzone
    * BUGFIX      #863 [AdminBundle]     Workaround for chrome rendering-bug of overlay in the content-edit
    * ENHANCEMENT #942 [ContactBundle]   Changed max characters of street from 60 to 150
    * BUGFIX      #905 [ContactBundle]   Added Functionality for completing contact addresses
    * FEATURE     #940 [ContactBundle]   Added command for fixing nested tree of accounts sulu:contacts:accounts:recover
    * BUGFIX      #876 [ContactBundle]   Bugfix contact adresses and replacing husky select with native select
    * FEATURE     #873 [ContactBundle]   Command-line data-completion-script: automatically set state of all
                                         account-addresses in database. 'app/console sulu:contacts:data:complete -d state'
    * BUGFIX      #908 [CategoryBundle]  Added script for recovering categories nested tree (fixing left/right and depths)
    * FEATURE     #838 [SecurityBundle]  AJAX-Login and resetting of password
    * FEATURE     #886 [AdminBundle]     Moved SuluVersionPass to Sulu\Compontents\Util to make it useable from webspace bundles
    * FEATURE     #838 [AdminBundle]     Login UI
    * FEATURE     #812 [MediaBundle]     Added nested collection API and UI
    * FEATURE     #812 [MediaBundle]     Implemented move collections
    * FEATURE     #805 [MediaBundle]     Implementing media move
    * FEATURE     #909 [MediaBundle]     Added scroll down pagination for collection
    * ENHANCEMENT #907 [ContentBundle]   Added ability to define custom homepage template
    * BUGFIX      #955 [ContentBundle]   Added webspace and locale to page in smart-content to load snippet in correct language

* 0.16.1 (2015-02-27)
    * HOTFIX      #880 [ContentBundle]   Fixed changelog if user and contact has not the same id
    * HOTFIX      #880 [AdminBundle]     Fixed user link if user and contact has not the same id
    * HOTFIX      #880 [ContentBundle]   Fixed content type time to allow empty time values
    * HOTFIX      #882 [ContentBundle]   Fixed deletion of referenced pages

* 0.16.0 (2015-02-24)
    * BUGFIX      #866 [ContactBundle]   Serialization group "select" for serializing system users
    * BUGFIX      #860 [AdminBundle]     Extended toolbar to accept more options
    * BUGFIX      #865 [ContentBundle]   Added validation and localized formatted value for time field
    * FEATURE     #413 [ClientBundle]    Added example for present as
    * BUGFIX      #848 [ContactBundle]   Refactored delete dialog function to make it reuseable
    * BUGFIX      #846 [MediaBundle]     Added missing dot to create event name method
    * ENHANCEMENT #841 [SecurityBundle]  Unique email per user
    * BUGFIX      #837 [AdminBundle]     Javascript function for croping labels with a certain tag this.sandbox.sulu.cropAllLabels(className)
    * ENHANCEMENT #818 [ContentBundle]   Enhanced column-navigation ordering ui
    * BUGFIX      #857 [ContentBundle]   Added links without save could not be removed
    * FEATURE     #789 [ContentBundle]   Added present as to smart content config (see [here ...](https://github.com/sulu-cmf/docs/blob/master/developer-documentation/300-webspaces/smart-content.md))
    * BUGFIX      #856 [ContentBundle]   Added default values for smart content view vars

* 0.15.3 (2015-02-19)
    * BUGFIX      #846 [MediaBundle]     Added missing dot to create event name method (\cc Daniel)

* 0.15.2 (2015-02-19)
    * HOTFIX      #850 [MediaBundle]     Fixed bug with deleted media in media selection

* 0.15.1 (2015-02-17)
    * HOTFIX      #842 [CoreBundle]      Fixed upgrade internal links command for installations without snippets

* 0.15.0 (2015-02-13)
    * FEATURE     #405 [sulu-standard]   Inclusion of PHPCR-Shell as a dev dependency
    * ENHANCEMENT #401 [sulu-standard]   Using the SYMONY_ENV environment variable instead of APP_ENV
    * BUGFIX      #829 [ContactBundle]   Account-Contacts: show full-name of contact
    * ENHANCEMENT #828 [ContactBundle]   Changed columns for contact list and made concatenated columns not sortable
    * BUGFIX      #825 [WebsiteBundle]   Fixed syntax error in ExceptionController
    * FEATURE     #806 [SnippetBundle]   added sorting feature to snippet content type
    * FEATURE     #806 [ContentBundle]   added sorting feature to internal links content type
    * ENHANCEMENT #798 [All]             Updated Symfony version to 2.6
    * BUGFIX      #826 [All]             Moved locales config from admin-bundle to core-bundle
    * BUGFIX      #736 [WebsiteBundle]   Redirect with port didn't work
    * ENHANCEMENT #735 [CategoryBundle]  Use parameters instead of FCQN of entities in service config
    * ENHANCEMENT #735 [MediaBundle]     Use parameters instead of FCQN of entities in service config
    * ENHANCEMENT #735 [TagBundle]       Use parameters instead of FCQN of entities in service config
    * FEATURE     #792 [ContactBundle]   added widget to show all companys of contact
    * FEATURE     #820 [ContactBundle]   Contact-Import: define multiple tags: 'account_tag1 ..n'
    * FEATURE     #810 [ContactBundle]   added command line tool for detecting missing country codes in import csv files
                                         that uses google geo api for finding the correct country code
    * BUGFIX      #801 [All]             Removed unused clean task which is deleting the public directory when executed
                                         due to the symfony 2.6 changes to symlinks
    * FEATURE     #793 [SecurityBundle]  Added field passwordForgetToken to BaseUser-Entity
    * FEATURE     #793 [ContactBundle]   Added Repository service for Contact
    * BUGFIX      #795 [ContentBundle]   Reversed structure paths to enable custom config
    * ENHANCEMENT #776 [CoreBundle]      Added set title to index page for init webspaces
    * BUGFIX      #774 [ContentBundle]   Enabled save shadow for index pages
    * BUGFIX      #778 [ContentBundle]   Fixed shadow page with internal link and smart-content
    * BUGFIX      #790 [WebsiteBundle]   Fixed twig variables for 404 page
    * FEATURE     #684 [ContentBundle]   Refactored preview to use new websocket component and only one socket for form
                                         and preview
    * FEATURE     #684 [WebsocketBundle] Implemented Websocket Component to standardize Websocket implementations
    * BUGFIX      #753 [MediaBundle]     Fix 0 bytes file upload
    * FEATURE     #714 [ContentBundle]   Add Option to hide page in sidemap
    * ENHANCEMENT #740 [SecurityBundle]  Made role content navigation extendable
    * FEATURE     #569 [All]             Behat integration - behat features for bundles
    * ENHANCEMENT #692 [SecurityBundle]  Made user extendable
    * ENHANCEMENT #731 [TestBundle]      Removed test user
    * BUGFIX      #671 [MediaBundle]     Fixed fileversion update with meta data
    * FEATURE     #702 [AdminBundle]     Added sortings to user settings and changed default url for activities
    * BUGFIX      #697 [ContactBundle]   Set VAT number field optional
    * BUGFIX      #697 [CoreBundle]      Do not try and set the theme when the portal has not been found
    * FEATURE     #697 [HttpCacheBundle] Refactored HTTP cache, introduced Varnish support. See 38af8da73c929f9f57bb87a8973a1ee55dccee29
    * ENHANCEMENT #777 [ContentBundle]   Enable "copy language" on startpage
    * FEATURE     #722 [ClientBundle]    Add Dependency Injection
    * ENHANCEMENT #699 [sulu-standard]   Add single internal link and checkbox to example
    * ENHANCEMENT #404 [AdminBundle]     Added config param "sulu_admin.locales" for content locales

* 0.14.2 (2015-02-02)
    * HOTFIX      #781 [CoreBundle]     HTTP Cache event listener uses the wrong event name due to recent change

* 0.14.1 (2015-01-21)
    * HOTFIX      #741 [ContentBundle]  Fix Resourcelocater Content Type call move without editing
    * HOTFIX      #737 [MediaBundle]    Changed BaseCollection properties to be protected for inheritance

* 0.14.0 (2015-01-15)
    * ENHANCEMENT #695 [ContentBundle]  Hide textblock sort option when there is only 1 textblock available
    * FEATURE     #634 [AdminBundle]    Created new configuration component, added new configuration for autocomplete
    * BUGFIX      #681 [TagBundle]      Fixed filtering of tags in Tag list and Media edit Overlay
    * BUGFIX      #681 [MediaBundle]    Fixed imagick detection
    * FEATURE     #581 [SearchBundle]   Structures deindexed on delete
    * FEATURE     #581 [Content]        NODE_SAVE renamed to NODE_POST_SAVE
    * FEATURE     #581 [Content]        New events: NODE_PRE_DELETE, NODE_POST_DELETE
    * FEATURE     #634 [AdminBundle]    Created new configuration component, added new configuration for autocomplete
                                        and refactored usage of autocomplete
    * BUGFIX      #627 [ContentBundle]  Fixed damaged urls when moving/copy/rename
    * ENHANCEMENT #639 [AdminBundle]    Save page size for datagrid
    * FEATURE     #659 [MediaBundle]    Configurable image quality settings
    * ENHANCEMENT #644 [AdminBundle]    Displaying an error label everytime a request fails
    * ENHANCEMENT #665 [SecurityBundle] Added role creation command and question for role in user creation
    * FEATURE     #662 [SnippetBundle]  Applied security
    * FEATURE     #662 [CategoryBundle] Applied security
    * FEATURE     #662 [TagBundle]      Applied security
    * BUGFIX      #654 [ContentBundle]  Added dummy request to request stack for preview rendering.
                                        This is important when template uses ESI
    * BUGFIX      #661 [WebsiteBundle]  Added published date to resolver
    * BUGFIX      #655 [ContentBundle]  Fixed checkbox read for preview

* 0.13.2 (2014-12-12)

    * HOTFIX      #--- [AdminBundle]    Fixed globalize loading issue
    * HOTFIX      #--- [AdminBundle]    Fixed datagrid destroy method (remove window resize listener)

* 0.13.1 (2014-12-11)
    * HOTFIX      #--- [AdminBundle]    Added missing frontend (css/js) build

* 0.13.0 (2014-12-10)

    * HOTFIX      #619 [MediaBundle]    Made web folder for format cache configurable
    * FEATURE     #637 [WebsiteBundle]  Multisort method and Twig filter
    * FEATURE     #585 [ContentBundle]  Added analytics key to webspace configuration
    * BUGFIX      #612 [SnippetBundle]  Introduced snippet pagination
    * BUGFIX      #544 [ContentBundle]  Fixed PHPCR Format Value switches
    * ENHANCEMENT #599 [ContentBundle]  Moved cache for preview from phpcr to filesystem
    * BUGFIX      #632 [SecurityBundle] Fixed language changer for admin
    * BUGFIX      #633 [SnippetBundle]  Load snippets always in requested language (except there is no translation and
                                        the page is a shadow then use this language)
* 0.12.0 (2014-11-25)

    * HOTFIX      #594 [WebsiteBundle]  Fixed sitemap alternate link bugs
    * BUGFIX      #609 [All]            Allows null value for security subject and fixed snippet internal links bug
    * ENHANCEMENT #577 [All]            Applied security to navigation items and content tabs
    * ENHANCEMENT #604 [CoreBundle]     Only register services for the current context
    * ENHANCEMENT #--- [Tests]          Fixed output colors for Mac users
    * BUGFIX      #571 [CoreBundle]     Fixed build command
    * ENHANCEMENT #556 [MediaBundle]    Enhanced url generation for collections
    * ENHANCEMENT #535 [SecurityBundle] Added SecurityListener and secured Content, Media and Security
    * BUGFIX      #568 [SnippetBundle]  Added template to view for Snippets
    * ENHANCEMENT #539 [AdminBundle]    Added validation for iban and vat numbers from the eu
    * HOTFIX      #559 [CoreBundle]     Workaround upstream reg. in DoctrinePHPCRBundle, which causes
                                        eager validation of workspace existence.
    * ENHANCEMENT #523 [All]            Refactored and improved functional tests
    * FEATURE     #553 [SnippetBundle]  Possiblity to show all snippet types by not providing any
    * BUGFIX      #533 [CoreBundle]     Removed request_analyzer.enable option (it is now irrelevant)
    * FEATURE     #563 [CoreBundle]     Introduced LocalizationProviders to offer the possibility to
    * BUGFIX      #563 [SecurityBundle] Showing correct localizations in UserRole-Assignment in
                                        Permission-Tab
    * FEATURE     #564 [ContentBundle]  Added UI to copy content languages
    * HOTFIX      #559 [CoreBundle]     Workaround upstream reg. in DoctrinePHPCRBundle, which causes
                                        eager validation of workspace existence.
    * ENHANCEMENT #523 [All]            Refactored and improved functional tests
    * BUGFIX      #597 [ContentBundle]  Reconnect to mysql if connection gone away in websocket
    * FEATURE     #368 [SnippetBundle]  Added `sulu:snippet:locale-copy`-command

* 0.11.2 (2014-11-17)

    * HOTFIX #559 [CoreBundle]    Workaround upstream reg. in DoctrinePHPCRBundle, which causes
                                  eager validation of workspace existence.
* 0.11.1 (2014-11-13)

    * HOTFIX #543 [SearchBundle]  Fixed re-index command
    * HOTFIX #551 [SearchBundle]  Switched to test adapter for tests
    * HOTFIX #549 [ContentBundle] Fixed page URL fetching for internal links used in snippets
    * HOTFIX #512 [MediaBundle]   Only show Media from specific selected Collection
    * HOTFIX #550 [MediaBundle]   Deleted Media do not throw Exception when page is saved

* 0.11.0 (2014-11-12)

    * BUGFIX      #540                 Real url in requested language (navigation, ...) for shadows
    * ENHANCEMENT #523 [ContentBundle] Prefix ContentBundle template path
    * BUGFIX      #531 [ContentBundle] Fixed single internal link freeze
    * BUGFIX      #529 [MediaBundle]   Display sorted Collections in overlay
    * FEATURE     #536 [MediaBundle]   Added Configurable display options for media-selection
    * ENHANCEMENT #361 [WebsiteBundle] Read urls for pages in all languages
    * ENHANCEMENT #526 [WebsiteBundle] Added Template var to resolver (Twig-Template)
    * ENHANCEMENT #528 [WebsiteBundle] Added memoize service to cache data and use it in twig extension
    * ENHANCEMENT #524 [ContentBundle] Prefix ContentBundle template path
    * BUGFIX      #518 [ContentBundle] Ordering of page changed when node is renamed
    * FEATURE     #511 [SnippetBundle] Ask confirmation when deleting Snippets which are referenced by content

* 0.10.2 (2014-11-07)

    * HOTFIX #509 [ContentBundle] Fixed cached data bug in smart-content

* 0.10.1 (2014-11-04)

* 0.10.0 (2014-11-03)
