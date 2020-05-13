# NHL-Api
download team and player data from https://statsapi.web.nhl.com/

all teams link : https://statsapi.web.nhl.com/api/v1/teams

sample data format

{
  "copyright" : "NHL and the NHL Shield are registered trademarks of the National Hockey League. NHL and NHL team marks are the property of the NHL and its teams. © NHL 2020. All Rights Reserved.",
  "teams" : [ {
    "id" : 1,
    "name" : "New Jersey Devils",
    "link" : "/api/v1/teams/1",
    "venue" : {
      "name" : "Prudential Center",
      "link" : "/api/v1/venues/null",
      "city" : "Newark",
      "timeZone" : {
        "id" : "America/New_York",
        "offset" : -4,
        "tz" : "EDT"
      }
    },
    "abbreviation" : "NJD",
    "teamName" : "Devils",
    "locationName" : "New Jersey",
    "firstYearOfPlay" : "1982",
    "division" : {
      "id" : 18,
      "name" : "Metropolitan",
      "nameShort" : "Metro",
      "link" : "/api/v1/divisions/18",
      "abbreviation" : "M"
    },
    "conference" : {
      "id" : 6,
      "name" : "Eastern",
      "link" : "/api/v1/conferences/6"
    },
    "franchise" : {
      "franchiseId" : 23,
      "teamName" : "Devils",
      "link" : "/api/v1/franchises/23"
    },
    "shortName" : "New Jersey",
    "officialSiteUrl" : "http://www.newjerseydevils.com/",
    "franchiseId" : 23,
    "active" : true
  }
  
  
individual player from roster data sample link : https://statsapi.web.nhl.com/api/v1/teams/1/roster

sample data format

{
  "copyright" : "NHL and the NHL Shield are registered trademarks of the National Hockey League. NHL and NHL team marks are the property of the NHL and its teams. © NHL 2020. All Rights Reserved.",
  "roster" : [ {
    "person" : {
      "id" : 8471233,
      "fullName" : "Travis Zajac",
      "link" : "/api/v1/people/8471233"
    },
    "jerseyNumber" : "19",
    "position" : {
      "code" : "C",
      "name" : "Center",
      "type" : "Forward",
      "abbreviation" : "C"
    }
  }
  
  
player stats sample link: https://statsapi.web.nhl.com/api/v1/people/8471233/stats?stats=statsSingleSeason&season=20192020

sample stat format:

{
  "copyright" : "NHL and the NHL Shield are registered trademarks of the National Hockey League. NHL and NHL team marks are the property of the NHL and its teams. © NHL 2020. All Rights Reserved.",
  "stats" : [ {
    "type" : {
      "displayName" : "statsSingleSeason"
    },
    "splits" : [ {
      "season" : "20192020",
      "stat" : {
        "timeOnIce" : "1179:36",
        "assists" : 16,
        "goals" : 9,
        "pim" : 28,
        "shots" : 72,
        "games" : 69,
        "hits" : 58,
        "powerPlayGoals" : 1,
        "powerPlayPoints" : 1,
        "powerPlayTimeOnIce" : "39:55",
        "evenTimeOnIce" : "942:36",
        "penaltyMinutes" : "28",
        "faceOffPct" : 52.84,
        "shotPct" : 12.5,
        "gameWinningGoals" : 1,
        "overTimeGoals" : 0,
        "shortHandedGoals" : 1,
        "shortHandedPoints" : 3,
        "shortHandedTimeOnIce" : "197:05",
        "blocked" : 39,
        "plusMinus" : -12,
        "points" : 25,
        "shifts" : 1476,
        "timeOnIcePerGame" : "17:05",
        "evenTimeOnIcePerGame" : "13:39",
        "shortHandedTimeOnIcePerGame" : "02:51",
        "powerPlayTimeOnIcePerGame" : "00:34"
      }
    } ]
  } ]
}
