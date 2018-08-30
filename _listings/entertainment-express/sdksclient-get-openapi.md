---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns a zip file of client SDK.
  description: Generate and download SDK's for using the API.  Requires a subscription
    key for authorization and a valid client.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analytics/City/:
    get:
      summary: Get Viewers by City.
      description: No required parameters, DateValue defaults to Today..
      operationId: GetAnalyticsViewersByCity
      x-api-path-slug: analyticscity-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - City
  /Analytics/Country/:
    get:
      summary: Get Viewers by Country.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByCountry
      x-api-path-slug: analyticscountry-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Country
  /Analytics/EngagementActions/:
    get:
      summary: GetAnalyticEngagementActions
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticEngagementActions
      x-api-path-slug: analyticsengagementactions-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - EngagementActions
  /Analytics/EngagementTimes/:
    get:
      summary: Get View count by Frequency.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsEngagementTimes
      x-api-path-slug: analyticsengagementtimes-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - EngagementTimes
  /Analytics/GBUsage/:
    get:
      summary: Get GBUsage by Customer ID.
      description: Requires a valid Customer ID.
      operationId: GetAnalyticsGBUsage
      x-api-path-slug: analyticsgbusage-get
      parameters:
      - in: query
        name: Month
        description: Report month
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Year
        description: Report year
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - GBUsage
  /Analytics/MostActive/:
    get:
      summary: Get Most Active Visitors by IP.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsMostActive
      x-api-path-slug: analyticsmostactive-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - MostActive
  /Analytics/PlatformHardware/:
    get:
      summary: Get Viewers by Platform Hardware.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByPlatformHardware
      x-api-path-slug: analyticsplatformhardware-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - PlatformHardware
  /Analytics/PlatformOS/:
    get:
      summary: Get Viewers by Platform OS.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByPlatformOS
      x-api-path-slug: analyticsplatformos-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - PlatformOS
  /Analytics/RecentVisitors/:
    get:
      summary: Get Most Recent Visitors by Time.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsRecentVisitors
      x-api-path-slug: analyticsrecentvisitors-get
      parameters:
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - RecentVisitors
  /Analytics/Summary/:
    get:
      summary: Get Summary by Customer ID.
      description: Requires a valid Customer ID.
      operationId: GetAnalyticsSummary
      x-api-path-slug: analyticssummary-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Summary
  /Analytics/TitleReport/:
    get:
      summary: Get Title Report by PublishedID.
      description: Requires a valid published ID.
      operationId: GetAnalyticsTitleReport
      x-api-path-slug: analyticstitlereport-get
      parameters:
      - in: query
        name: End
        description: Report end date
      - in: query
        name: PublishedId
        description: Title published ID
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - TitleReport
  /Analytics/VideoLog/:
    get:
      summary: Get Views by Video.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewsByVideoLog
      x-api-path-slug: analyticsvideolog-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - VideoLog
  /Analytics/Viewers/:
    get:
      summary: Get viewers by Day.
      description: Optional DateValue for length of report.
      operationId: GetAnalyticsViewers
      x-api-path-slug: analyticsviewers-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Viewers
  /Analytics/Views/:
    get:
      summary: Get views by Day.
      description: Optional DateValue for length of report.
      operationId: GetAnalyticsViews
      x-api-path-slug: analyticsviews-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Views
  /Analytics/WebBrowsers/:
    get:
      summary: Get Viewers by Web Browser.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByWebBrowsers
      x-api-path-slug: analyticswebbrowsers-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - WebBrowsers
  /Changes/Episodes/History/:
    get:
      summary: Returns list of unique EpisodeId changes greater than or equal to date
        (UTC)
      description: For each updated episode ID, pull the full episode data for that
        ID and update.
      operationId: GetEpisodeChangeHistory
      x-api-path-slug: changesepisodeshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - History
  /Changes/Episodes/HistoryWithEntity/:
    get:
      summary: Returns list of unique EpisodeId and Entity changes greater than or
        equal to date (UTC).
      description: Lists each episode ID that has changed as well as the entity in
        the object that changed.
      operationId: GetEpisodeChangeHistoryWithEntity
      x-api-path-slug: changesepisodeshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - HistoryWithEntity
  /Changes/Movies/History/:
    get:
      summary: Returns list of unique MovieId changes greater than or equal to date
        (UTC).
      description: Use to get the ID's of the movies that have been added or changed
        and use /Movies/{ID} to get back the object with the updated data and replace
        in your database.
      operationId: GetMovieChangeHistory
      x-api-path-slug: changesmovieshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Movies
      - History
  /Changes/Movies/HistoryWithEntity/:
    get:
      summary: Returns list of unique MovieId and Entity changes greater than or equal
        to date (UTC).
      description: Same as /Changes/Movies/History but with the specific entities
        that have changed inside the MovieResponse.
      operationId: GetMovieChangeHistoryWithEntity
      x-api-path-slug: changesmovieshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Movies
      - HistoryWithEntity
  /Changes/People/History/:
    get:
      summary: Returns list of unique PersonId changes greater than or equal to date
        (UTC).
      description: Requires a valid Date.
      operationId: GetPersonChangeHistory
      x-api-path-slug: changespeoplehistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - People
      - History
  /Changes/People/HistoryWithEntity/:
    get:
      summary: Returns list of unique PersonId and Entity changes greater than or
        equal to date (UTC).
      description: Requires a valid Date.
      operationId: GetPersonChangeHistoryWithEntity
      x-api-path-slug: changespeoplehistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - People
      - HistoryWithEntity
  /Changes/Seasons/History/:
    get:
      summary: Returns list of unique SeasonId changes greater than or equal to date
        (UTC).
      description: Use if you want to check for specific updates to season records.
      operationId: GetSeasonChangeHistory
      x-api-path-slug: changesseasonshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Seasons
      - History
  /Changes/Seasons/HistoryWithEntity/:
    get:
      summary: Returns list of unique SeasonId and Entity changes greater than or
        equal to date (UTC).
      description: Returns list of new or changed SeasonIds with the entity that has
        changed.
      operationId: GetSeasonChangeHistoryWithEntity
      x-api-path-slug: changesseasonshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Seasons
      - HistoryWithEntity
  /Changes/Shows/History/:
    get:
      summary: Returns list of unique ShowId changes greater than or equal to date
        (UTC).
      description: All new and updated shows from requested date and time.  When a
        record gets updated, use the ID to get the full show object and replace the
        data in your cache.
      operationId: GetShowChangeHistory
      x-api-path-slug: changesshowshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Shows
      - History
  /Changes/Shows/HistoryWithEntity/:
    get:
      summary: Returns list of unique ShowId and Entity changes greater than or equal
        to date (UTC).
      description: Returns a list of ShowId and entity of any show that has been updated.
      operationId: GetShowChangeHistoryWithEntity
      x-api-path-slug: changesshowshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Shows
      - HistoryWithEntity
  /Charts/Movies/Boxoffice:
    get:
      summary: Returns list of movies based on the weekend box office revenue.
      description: Returns top 10 box office movies.
      operationId: GetChartMoviesBoxoffice
      x-api-path-slug: chartsmoviesboxoffice-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - Boxoffice
  /Charts/Movies/MostAnticipated:
    get:
      summary: Returns list of Most Anticipated movies based on IVA data.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartMoviesMostAnticipated
      x-api-path-slug: chartsmoviesmostanticipated-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - MostAnticipated
  /Charts/Movies/Popular:
    get:
      summary: Returns list of popular movies.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartMoviesPopular
      x-api-path-slug: chartsmoviespopular-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - Popular
  /Charts/People/Popular:
    get:
      summary: Returns list of popular celebrities based on IVA data.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartPeoplePopular
      x-api-path-slug: chartspeoplepopular-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - People
      - Popular
  /Charts/Shows/Popular:
    get:
      summary: Returns a list of shows based on popularity.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartShowsPopular
      x-api-path-slug: chartsshowspopular-get
      parameters:
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Shows
      - Popular
  /Common/Companies/:
    get:
      summary: Paged list of companies.
      description: 'Companies are listed in a movie, show, or game response as those
        whom are involved with the program.  EX: Universal Pictures.'
      operationId: GetCompanies
      x-api-path-slug: commoncompanies-get
      parameters:
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Common
      - Companies
  /Common/Countries/:
    get:
      summary: Returns a list of countries.
      description: List of Countries, ISO codes and Country IDs used throughout the
        API.
      operationId: GetCountries
      x-api-path-slug: commoncountries-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - Countries
  /Common/ImageTypes/:
    get:
      summary: List of image types contained in the database.
      description: 'A list of image types available in the IVA database. **EX: Poster**'
      operationId: GetImageTypes
      x-api-path-slug: commonimagetypes-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - ImageTypes
  /Common/Languages/:
    get:
      summary: Gets all languages.
      description: Returns a list of languages used in the API as well as the ISO
        code and language ID.
      operationId: GetLanguages
      x-api-path-slug: commonlanguages-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - Languages
  /Common/Tags/:
    get:
      summary: Gets all tags.
      description: Paged list of all tags used in the API.
      operationId: GetTags
      x-api-path-slug: commontags-get
      parameters:
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Common
      - Tags
  /Common/VideoTypes/:
    get:
      summary: Gets all VideoTypes.
      description: Returns a list of the types of videos that can be associated to
        a title.
      operationId: GetVideoTypes
      x-api-path-slug: commonvideotypes-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - VideoTypes
  /ExternalIds/GracenoteMovie:
    get:
      summary: Returns list of all MovieId, Gracenote Id pairs.
      description: Not accessible with a Demo account.  **Special permissions needed**
        for access to this operation.  Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetGracenoteMovieIds
      x-api-path-slug: externalidsgracenotemovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - GracenoteMovie
  /ExternalIds/GracenoteShow:
    get:
      summary: Returns list of all ShowId, Gracenote Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetGracenoteShowIds
      x-api-path-slug: externalidsgracenoteshow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - GracenoteShow
  /ExternalIds/ImdbMovie:
    get:
      summary: Returns list of all MovieId, IMDB Id pairs.
      description: Ingest this ID map to create connections between the objects in
        your existing database with an IMDB ID to the IVA Movie objects.
      operationId: GetImdbMovieIds
      x-api-path-slug: externalidsimdbmovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - ImdbMovie
  /ExternalIds/ImdbShow:
    get:
      summary: Returns list of all MovieId, Tmdb Id pairs.
      description: ngest this ID map to create connections between the objects in
        your existing database with an IMDB ID to the IVA Show objects.
      operationId: GetImdbShowIds
      x-api-path-slug: externalidsimdbshow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - ImdbShow
  /ExternalIds/RoviMovie:
    get:
      summary: Returns list of all MovieId, Tivo Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetTivoMovieIds
      x-api-path-slug: externalidsrovimovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - RoviMovie
  /ExternalIds/RoviShow:
    get:
      summary: Returns list of all ShowId, Tivo Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetTivoShowIds
      x-api-path-slug: externalidsrovishow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - RoviShow
  /ExternalIds/TmdbMovie:
    get:
      summary: Returns list of all MovieId, Tmdb Id pairs.
      description: Use to link a TMDB ID to an IVA Movie ID.
      operationId: GetTmdbMovieIds
      x-api-path-slug: externalidstmdbmovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - TmdbMovie
  /ExternalIds/TmdbShow:
    get:
      summary: Returns list of all ShowId, TMDB Id pairs.
      description: Use to link a TMDB ID to an IVA Show ID.
      operationId: GetTmdbShowIds
      x-api-path-slug: externalidstmdbshow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - TmdbShow
  /ExternalIds/Webedia:
    get:
      summary: Returns list of all MovieId, Webedia Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetWebediaMovieIds
      x-api-path-slug: externalidswebedia-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - Webedia
  /Find/Movie/:
    get:
      summary: Find a movie using third party ID.
      description: "Use FindMovie with a third party ID like IMDB, TMDB, Gracenote,
        Tivo, etc. to find the corresponding movie in the IVA database.  For a full
        list of supported ID types see /Movies/AlternateIdTypes. \n\n\n\n`Recommendation:
        Use with small data sets or for a proof of concept. `"
      operationId: FindMovie
      x-api-path-slug: findmovie-get
      parameters:
      - in: query
        name: Id
        description: Required third party ID of Movie
      - in: query
        name: IdType
        description: Required third party ID type of MovieAlternateId
      - in: query
        name: Includes
        description: List of additional objects to include in the movie object
      responses:
        200:
          description: OK
      tags:
      - Find
      - Movie
  /Find/Show/:
    get:
      summary: Find a TV show using a third party ID.
      description: 'Use FindShow with a third party ID like IMDB, TMDB, Gracenote,
        Tivo, etc. to find the corresponding TV show in the IVA database. For a full
        list of supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use
        with small data sets or for a proof of concept. `'
      operationId: FindShow
      x-api-path-slug: findshow-get
      parameters:
      - in: query
        name: Id
        description: Required third party ID of Show
      - in: query
        name: IdType
        description: Required third party ID type of ShowAlternateId
      - in: query
        name: Includes
        description: List of additional objects to include in the show response
      responses:
        200:
          description: OK
      tags:
      - Find
      - Show
  /GoWatchIt/Episodes/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Episode Availability.
      description: Returns GoWatchit episode availability by Entertainment Episode
        ID. Special permission is required to access this endpoint.
      operationId: GetGoWatchItEpisodeAvailabilities
      x-api-path-slug: gowatchitepisodesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Episode
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Episodes
      - Id
      - Availabilities
  /GoWatchIt/Movies/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Movie Availability.
      description: Returns GoWatchIt movie availability by Entertainment Movie ID.  Special
        permission is required to access this endpoint.  Contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItMovieAvailabilities
      x-api-path-slug: gowatchitmoviesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Movie
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Movies
      - Id
      - Availabilities
  /GoWatchIt/Seasons/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Season Availability.
      description: Returns GoWatchIt season availability by Entertainment Season ID.  Special
        permission is required to access this endpoint.  Contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItSeasonAvailabilities
      x-api-path-slug: gowatchitseasonsidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Season
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Seasons
      - Id
      - Availabilities
  /GoWatchIt/Shows/{Id}/Availabilities:
    get:
      summary: Get GoWatchItShow Availability.
      description: Returns GoWatchIt show availability by Entertainment Show ID.  Special
        permission is required to access this endpoint. Please contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItShowAvailabilities
      x-api-path-slug: gowatchitshowsidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Show
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Shows
      - Id
      - Availabilities
  /Images/Batch:
    post:
      summary: Returns a list of batch image responses links based on filepath.
      description: Requires a list filepath.
      operationId: GetImageBatch
      x-api-path-slug: imagesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: FilePath
        description: List of Filepaths
      responses:
        200:
          description: OK
      tags:
      - Images
      - Batch
  /Images/ScreenCaptures/Batch:
    post:
      summary: Returns a list of screen capture responses.
      description: Requires a list of filepaths.
      operationId: GetScreenCaptureBatch
      x-api-path-slug: imagesscreencapturesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: FilePath
        description: List of Filepaths
      responses:
        200:
          description: OK
      tags:
      - Images
      - ScreenCaptures
      - Batch
  /Images/ScreenCaptures/Redirect:
    get:
      summary: Redirect to a screen capture based on filepath.
      description: "Requires a valid filepath of a video asset screen capture.  \n\n`Note:
        The swagger U/I does not support redirects.`"
      operationId: GetScreenCapture
      x-api-path-slug: imagesscreencapturesredirect-get
      parameters:
      - in: query
        name: FilePath
        description: Filepath of Image
      - in: query
        name: Redirect
        description: Redirect to the image
      responses:
        200:
          description: OK
      tags:
      - Images
      - ScreenCaptures
      - Redirect
  /Images/{FilePath}/Redirect:
    get:
      summary: Redirect to an image based on filepath.
      description: "Images should be downloaded and stored on the client server. Use
        /Common/ImageTypes to see a list of available image types.  \n\n\n`Note: The
        swagger U/I does not support redirects.`"
      operationId: GetImage
      x-api-path-slug: imagesfilepathredirect-get
      parameters:
      - in: path
        name: FilePath
        description: Filepath of Image
      - in: query
        name: Redirect
        description: Redirect to the image
      responses:
        200:
          description: OK
      tags:
      - Images
      - FilePath
      - Redirect
  /Metacritic/Movie/{Id}:
    get:
      summary: Get Metacritic Movie information.
      description: Returns Metacritic Movie information by Entertainment Movie ID.
      operationId: GetMetacriticMovie
      x-api-path-slug: metacriticmovieid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Entertainment Movie
      responses:
        200:
          description: OK
      tags:
      - Metacritic
      - Movie
      - Id
  /Metacritic/TV/{Id}:
    get:
      summary: Get Metacritic TV information.
      description: Returns Metacritic TV information by Entertainment Show ID.
      operationId: GetMetacriticTv
      x-api-path-slug: metacritictvid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Entertainment Show
      - in: query
        name: SeasonNumber
        description: Number of season
      responses:
        200:
          description: OK
      tags:
      - Metacritic
      - TV
      - Id
  /MovieTickets/Cultures:
    get:
      summary: Get MovieTickets Cultures.
      description: Returns MovieTickets Cultures.
      operationId: GetMovieTicketsCultures
      x-api-path-slug: movieticketscultures-get
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Cultures
  /MovieTickets/Movies/ComingSoon:
    get:
      summary: Get MovieTickets Movies releasing soon.
      description: Returns MovieTickets Movies releasing soon.
      operationId: GetMovieTicketsMoviesComingSoon
      x-api-path-slug: movieticketsmoviescomingsoon-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: PageNumber
        description: Page number for paging results
      - in: query
        name: PageSize
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Movies
      - ComingSoon
  /MovieTickets/Movies/NowPlaying:
    get:
      summary: Get MovieTickets Movies in theaters.
      description: Returns MovieTickets Movies currently in theaters.
      operationId: GetMovieTicketsMoviesNowPlaying
      x-api-path-slug: movieticketsmoviesnowplaying-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: PageNumber
        description: Page number for paging results
      - in: query
        name: PageSize
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Movies
      - NowPlaying
  /MovieTickets/Performances:
    get:
      summary: Get MovieTickets Performances.
      description: Returns MovieTickets Performances by MovieTickets Theater ID, Entertainment
        Movie ID, and ScheduleDate.
      operationId: GetMovieTicketsPerformances
      x-api-path-slug: movieticketsperformances-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: EntertainmentMovieIds
        description: Required ID/IDs of Entertainment Movies
      - in: query
        name: ScheduleDate
        description: Date to get scheduled performances
      - in: query
        name: TheaterIds
        description: Required ID/IDs of MovieTickets Theaters
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Performances
  /MovieTickets/Theaters:
    get:
      summary: Get MovieTickets Theaters.
      description: Returns MovieTickets Theaters by postal code.
      operationId: GetMovieTicketsTheaters
      x-api-path-slug: movieticketstheaters-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: Distance
        description: Required distaince in meters
      - in: query
        name: Latitude
        description: Latitude coordinate
      - in: query
        name: Longitude
        description: Longitude coordinate
      - in: query
        name: PageNumber
        description: Page number for paging results
      - in: query
        name: PageSize
        description: Limits the total items returned
      - in: query
        name: PostalCode
        description: Postal code
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Theaters
  /Movies/All:
    get:
      summary: Returns a paged list of all movies.
      description: "By default the API will only return basic title information. Additional
        objects can be included by passing the object in the Includes parameter.   \n\n\n`Subscriptions
        with \"Limited\" data will only be able to include basic title information
        and Videos.`"
      operationId: GetAllMovies
      x-api-path-slug: moviesall-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie objectSearch
          movie by OriginalTitle
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - Movies
  /Movies/AlternateIdTypes:
    get:
      summary: Returns all MovieAlternateIdTypes.
      description: "Movie alternate ID types refer to 3rd party IDs that IVA matches
        its own movie IDs.  **EX: IMDB, TMDB**.  \n\n`Use to get the Id of the ID
        type to use with /Find/Movie.`"
      operationId: GetMovieAlternateIdTypes
      x-api-path-slug: moviesalternateidtypes-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - AlternateIdTypes
  /Movies/ComingSoon/:
    get:
      summary: Returns list of all Movies coming to US Theaters.
      description: |-
        Requires Skip and Take. Maximum page size is 10.

        By default the API will only return basic title information.
        Additional objects can be included by passing the object in the Includes parameter in a comma separated list.
      operationId: GetMoviesComingSoon
      x-api-path-slug: moviescomingsoon-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Movies
      - ComingSoon
  /Movies/InTheaters/:
    get:
      summary: Returns list of all Movies currently in US Theaters.
      description: |-
        Requires Skip and Take. Maximum page size is 10.

        By default the API will only return basic title information.
        Additional objects can be included by passing the object in the Includes parameter in a comma separated list.
      operationId: GetMoviesInTheaters
      x-api-path-slug: moviesintheaters-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Movies
      - InTheaters
  /Movies/Match/:
    get:
      summary: Perform a match to Entertainment using Title, Year, Cast and Director.
        Returns best match and score for the match.
      description: Use to match IVA movie data to another data source using title,
        year, cast etc.
      operationId: MatchToMovie
      x-api-path-slug: moviesmatch-get
      parameters:
      - in: query
        name: AlternateTitles
        description: Alternate Titles of movie to be matched
      - in: query
        name: Cast
        description: Cast members of movie to be matched
      - in: query
        name: Directors
        description: Directors of movie to be matched
      - in: query
        name: StringDistance
        description: For fuzzy title match, default is 4, set to 0 for no fuzzy match
      - in: query
        name: Title
        description: Title of movie to be matched
      - in: query
        name: Year
        description: Release Year of movie to be matched
      responses:
        200:
          description: OK
      tags:
      - Movies
      - Match
  /Movies/MovieCertifications:
    get:
      summary: Returns all Movie Certifications
      description: Returns all Movie Certifications used in a movie response with
        the Releases object.
      operationId: GetMovieCertifications
      x-api-path-slug: moviesmoviecertifications-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - MovieCertifications
  /Movies/MovieGenres:
    get:
      summary: Returns all Movie Genres.
      description: List of all movie genres used in the API.
      operationId: GetMovieGenres
      x-api-path-slug: moviesmoviegenres-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - MovieGenres
  /Movies/ReleaseTypes:
    get:
      summary: Returns all Movie ReleaseTypes
      description: 'Release type refers to the release. **EX: Theatrical, Home Video,
        etc.**'
      operationId: GetMovieReleaseTypes
      x-api-path-slug: moviesreleasetypes-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - ReleaseTypes
  /Movies/SearchAndDiscover:
    get:
      summary: Search and discover movies.
      description: |-
        Searchable Fields:
        Title, AlternateTitles, Genres, OriginalReleaseDate, UnitedStatesReleaseDate, GermanyReleaseDate, FranceReleaseDate, UnitedKingdomReleaseDate, ItalyReleaseDate, JapanReleaseDate, Tags, Cast, Directors, Descriptions, Ratings, OriginalLanguage.
        [Syntax Ref](https://docs.microsoft.com/en-us/rest/api/searchservice/simple-query-syntax-in-azure-search)

        Filterable Fields:
        ID, Title, AlternateTitles, Genres, OriginalReleaseDate, UnitedStatesReleaseDate, GermanyReleaseDate, FranceReleaseDate, UnitedKingdomReleaseDate, ItalyReleaseDate, JapanReleaseDate, Year, Tags, Cast, Directors, Descriptions, HasVideo, PosterFilePath, Ratings, OriginalLanguage, Runtime, Budget, Revenue, Created, Modified.
        [Syntax Ref](https://docs.microsoft.com/en-us/rest/api/searchservice/odata-expression-syntax-for-azure-search)
      operationId: SearchAndDiscoverMovie
      x-api-path-slug: moviessearchanddiscover-get
      parameters:
      - in: query
        name: Filter
        description: Expression to filter results
      - in: query
        name: IncludeTotalResultCount
        description: Includes total results in response
      - in: query
        name: OrderBy
        description: List of field names to sort results
      - in: query
        name: SearchFields
        description: List of field names to search using term
      - in: query
        name: SearchMode
        description: Specifies whether ANY or ALL of the search terms must be matched
          in order to count the item as a match
      - in: query
        name: SelectFields
        description: List of field names to be returned in the object
      - in: query
        name: Skip
        description: Skip number of results
      - in: query
        name: term
        description: Term to search for
      - in: query
        name: Top
        description: Limit results
      responses:
        200:
          description: OK
      tags:
      - Movies
      - SearchAndDiscover
  /Movies/{Id}:
    get:
      summary: Returns movie data for a specific IVA MovieId.
      description: "By default the API will only return basic title information. Additional
        objects can be included by passing the object in the Includes parameter.   \n\n\n`Subscriptions
        with \"Limited\" data will only be able to include basic title information
        and Videos.`"
      operationId: GetMovie
      x-api-path-slug: moviesid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Movie
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      responses:
        200:
          description: OK
      tags:
      - Movies
      - Id
  /People/All:
    get:
      summary: Gets all People.
      description: Returns a AllPeopleResponse object containing a list of all poeple.
      operationId: GetAllPeople
      x-api-path-slug: peopleall-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the person response
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - People
  /People/RankedSearch/:
    get:
      summary: Find Person by Name ordered by rank.
      description: Find person using name ordered by rank.
      operationId: GetPersonRankedSearch
      x-api-path-slug: peoplerankedsearch-get
      parameters:
      - in: query
        name: StartsWith
      responses:
        200:
          description: OK
      tags:
      - People
      - RankedSearch
  /People/{Id}:
    get:
      summary: Returns information on a person.
      description: BETA - By default the API will only return basic People information.
        Additional objects can be included by passing the object in the Includes parameter.
      operationId: GetPerson
      x-api-path-slug: peopleid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Person
      - in: query
        name: Includes
        description: List of additional objects to include in the person response
      responses:
        200:
          description: OK
      tags:
      - People
      - Id
  /People/{Id}/Filmography:
    get:
      summary: Get a Person's Filmography.
      description: Requires a valid Person ID.
      operationId: GetFilmography
      x-api-path-slug: peopleidfilmography-get
      parameters:
      - in: path
        name: Id
      responses:
        200:
          description: OK
      tags:
      - People
      - Id
      - Filmography
  /SDKs/{Client}:
    get:
      summary: Returns a zip file of client SDK.
      description: Generate and download SDK's for using the API.  Requires a subscription
        key for authorization and a valid client.
      operationId: GetSDK
      x-api-path-slug: sdksclient-get
      parameters:
      - in: path
        name: Client
        description: Client SDK
      - in: query
        name: RedirectToFile
        description: Redirect to download the zipped SDK
      responses:
        200:
          description: OK
      tags:
      - SDKs
      - Client
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---