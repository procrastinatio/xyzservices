Changelog
=========

xyzservices 2021.11.0 (November 06, 2021)
----------------------------------------

Providers:

- Updated deprecated links to ``nlmaps`` providers
- Added ``nlmaps.water``


xyzservices 2021.10.0 (October 19, 2021)
----------------------------------------

Providers:

- Added ``OPNVKarte`` map
- Removed discontinued ``OpenPtMap``
- Max zoom of ``CartoDB`` tiles changed from 19 to 20


xyzservices 2021.09.1 (September 20, 2021)
------------------------------------------

New functionality:

- Added ``Bunch.query_name()`` method allowing to fetch the ``TileProvider`` object based on the name with flexible formatting. (#93)


xyzservices 2021.09.0 (September 3, 2021)
-----------------------------------------

Providers:

- Fixed ``Strava`` maps (#85)
- Fixed ``nlmaps.luchtfoto`` (#90)
- Fixed ``NASAGIBS.ModisTerraSnowCover`` (#90)
- ``JusticeMap`` and ``OpenAIP`` now use https instead of http


xyzservices 2021.08.1 (August 12, 2021)
---------------------------------------

Providers:

- Added ``OpenStreetMap.BlackAndWhite`` (#83)
- Added ``Gaode`` tiles (``Normal`` and ``Satellite``) (#83)
- Expanded ``NASAGIBS`` tiles with ``ModisTerraBands721CR``, ``ModisAquaTrueColorCR``, ``ModisAquaBands721CR`` and ``ViirsTrueColorCR`` (#83)
- Added metadata to ``Strava`` maps (currently down) (#83)


xyzservices 2021.08.0 (August 8, 2021)
--------------------------------------

New functionality:

- Added ``TileProvider.from_qms()`` allowing to create a ``TileProvider`` object from the remote [Quick Map Services](https://qms.nextgis.com/about) repository (#71)
- Added support of ``html_attribution`` to have live links in attributions in HTML-based outputs like leaflet (#60)
- New ``Bunch.flatten`` method creating a flat dictionary of ``TileProvider`` objects based on a nested ``Bunch`` (#68)
- Added ``fill_subdomain`` keyword to ``TileProvider.build_url`` to control ``{s}`` placeholder in the URL (#75)
- New Bunch.filter method to filter specific providers based on keywords and other criteria (#76)

Minor enhancements:

- Indent providers JSON file for better readability (#64)
- Support dark themes in HTML repr (#70)
- Mark broken providers with ``status="broken"`` attribute (#78)
- Document providers requiring registrations (#79)


xyzservices 2021.07 (July 30, 2021)
-----------------------------------

The initial release provides ``TileProvider`` and ``Bunch`` classes and an initial set of providers.
