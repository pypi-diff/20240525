# Comparing `tmp/pulsefire-types-2.0.8.tar.gz` & `tmp/pulsefire-types-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsefire-types-2.0.8.tar", last modified: Fri Mar  1 15:30:26 2024, max compression
+gzip compressed data, was "pulsefire-types-2.0.9.tar", last modified: Thu Apr 11 00:43:14 2024, max compression
```

## Comparing `pulsefire-types-2.0.8.tar` & `pulsefire-types-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:30:26.541639 pulsefire-types-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-01 15:30:26.541639 pulsefire-types-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-01 15:30:24.000000 pulsefire-types-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:30:26.537639 pulsefire-types-2.0.8/pulsefire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/pulsefire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67203 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/pulsefire/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:30:26.541639 pulsefire-types-2.0.8/pulsefire_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-01 15:30:26.000000 pulsefire-types-2.0.8/pulsefire_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-01 15:30:26.000000 pulsefire-types-2.0.8/pulsefire_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 15:30:26.000000 pulsefire-types-2.0.8/pulsefire_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 15:30:26.000000 pulsefire-types-2.0.8/pulsefire_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 15:30:26.000000 pulsefire-types-2.0.8/pulsefire_types.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 15:30:26.541639 pulsefire-types-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-01 15:30:24.000000 pulsefire-types-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:30:26.541639 pulsefire-types-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/tests/test_caches.py
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/tests/test_doc_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/tests/test_ratelimiters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-01 15:30:21.000000 pulsefire-types-2.0.8/tests/test_taskgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:43:14.449270 pulsefire-types-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-11 00:43:14.449270 pulsefire-types-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-11 00:43:11.000000 pulsefire-types-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:43:14.445270 pulsefire-types-2.0.9/pulsefire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/pulsefire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68887 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/pulsefire/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:43:14.449270 pulsefire-types-2.0.9/pulsefire_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-11 00:43:14.000000 pulsefire-types-2.0.9/pulsefire_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 00:43:14.000000 pulsefire-types-2.0.9/pulsefire_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:43:14.000000 pulsefire-types-2.0.9/pulsefire_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 00:43:14.000000 pulsefire-types-2.0.9/pulsefire_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:43:14.000000 pulsefire-types-2.0.9/pulsefire_types.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:43:14.449270 pulsefire-types-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-11 00:43:11.000000 pulsefire-types-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:43:14.449270 pulsefire-types-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/tests/test_caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/tests/test_doc_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/tests/test_ratelimiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-11 00:43:05.000000 pulsefire-types-2.0.9/tests/test_taskgroups.py
```

### Comparing `pulsefire-types-2.0.8/LICENSE` & `pulsefire-types-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pulsefire-types-2.0.8/PKG-INFO` & `pulsefire-types-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsefire-types
-Version: 2.0.8
+Version: 2.0.9
 Summary: A modern and flexible Riot Games Python SDK.
 Home-page: https://github.com/iann838/pulsefire
 Author: Jian Huang
 Author-email: iann838dev@gmail.com
 License: MIT
 Keywords: Riot Games,League of Legends,Teamfight Tactics,Valorant,Legends of Runeterra,API,SDK,asyncio
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pulsefire-types-2.0.8/README.md` & `pulsefire-types-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulsefire-types-2.0.8/pulsefire/schemas.py` & `pulsefire-types-2.0.9/pulsefire/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,28 +662,28 @@
         "losses": int,
         "progress": str,
         "target": int,
         "wins": int,
     })
     LolLeagueV4LeagueEntry = TypedDict("LolLeagueV4LeagueEntry", {
         "summonerId": str,
-        "summonerName": str,
+        "summonerName": NotRequired[str],
         "rank": str,
         "leaguePoints": int,
         "wins": int,
         "losses": int,
         "hotStreak": bool,
         "veteran": bool,
         "freshBlood": bool,
         "inactive": bool,
     })
     LolLeagueV4LeagueFullEntry = TypedDict("LolLeagueV4LeagueFullEntry", {
         "leagueId": str,
         "summonerId": str,
-        "summonerName": str,
+        "summonerName": NotRequired[str],
         "queueType": str,
         "tier": str,
         "rank": str,
         "leaguePoints": int,
         "wins": int,
         "losses": int,
         "hotStreak": bool,
@@ -867,19 +867,33 @@
         "playerScore4": float,
         "playerScore5": float,
         "playerScore6": float,
         "playerScore7": float,
         "playerScore8": float,
         "playerScore9": float,
     })
+    LolMatchV5MatchInfoParticipantMissionsAlt = TypedDict("LolMatchV5MatchInfoParticipant", {
+        "PlayerScore0": float,
+        "PlayerScore1": float,
+        "PlayerScore10": float,
+        "PlayerScore11": float,
+        "PlayerScore2": float,
+        "PlayerScore3": float,
+        "PlayerScore4": float,
+        "PlayerScore5": float,
+        "PlayerScore6": float,
+        "PlayerScore7": float,
+        "PlayerScore8": float,
+        "PlayerScore9": float,
+    })
     LolMatchV5MatchInfoParticipant = TypedDict("LolMatchV5MatchInfoParticipant", {
         "allInPings": int,
         "assistMePings": int,
         "assists": int,
-        "baitPings": int,
+        "baitPings": NotRequired[int],
         "baronKills": int,
         "basicPings": int,
         "bountyLevel": int,
         "challenges": NotRequired[LolMatchV5MatchInfoParticipantChallenges | dict[str, int | float]],
         "champExperience": int,
         "champLevel": int,
         "championId": int,
@@ -927,15 +941,15 @@
         "largestCriticalStrike": int,
         "largestKillingSpree": int,
         "largestMultiKill": int,
         "longestTimeSpentLiving": int,
         "magicDamageDealt": int,
         "magicDamageDealtToChampions": int,
         "magicDamageTaken": int,
-        "missions": NotRequired[LolMatchV5MatchInfoParticipantMissions],
+        "missions": NotRequired[LolMatchV5MatchInfoParticipantMissions | LolMatchV5MatchInfoParticipantMissionsAlt],
         "needVisionPings": int,
         "neutralMinionsKilled": int,
         "nexusKills": int,
         "nexusLost": int,
         "nexusTakedowns": int,
         "objectivesStolen": int,
         "objectivesStolenAssists": int,
@@ -980,15 +994,15 @@
         "subteamPlacement": int,
         "summoner1Casts": int,
         "summoner1Id": int,
         "summoner2Casts": int,
         "summoner2Id": int,
         "summonerId": str,
         "summonerLevel": int,
-        "summonerName": str,
+        "summonerName": NotRequired[str],
         "teamEarlySurrendered": bool,
         "teamId": int,
         "teamPosition": str,
         "timeCCingOthers": int,
         "timePlayed": int,
         "totalAllyJungleMinionsKilled": int,
         "totalDamageDealt": int,
@@ -1047,15 +1061,16 @@
         "gameType": str,
         "gameVersion": str,
         "mapId": int,
         "participants": list[LolMatchV5MatchInfoParticipant],
         "platformId": str,
         "queueId": int,
         "teams": list[LolMatchV5MatchInfoTeam],
-        "tournamentCode": str
+        "tournamentCode": str,
+        "endOfGameResult": str
     })
     LolMatchV5Match = TypedDict("LolMatchV5Match", {
         "metadata": LolMatchV5MatchMetadata,
         "info": LolMatchV5MatchInfo
     })
     LolMatchV5MatchTimelineParticipantFrameChampionStats = TypedDict("LolMatchV5MatchTimelineParticipantFrameChampionStats", {
         "abilityHaste": int,
@@ -1165,15 +1180,16 @@
         "participantId": int,
         "puuid": str,
     })
     LolMatchV5MatchTimelineInfo = TypedDict("LolMatchV5MatchTimelineInfo", {
         "frameInterval": int,
         "frames": list[LolMatchV5MatchTimelineInfoFrame],
         "gameId": int,
-        "participants": list[LolMatchV5MatchTimelineInfoParticipants]
+        "participants": list[LolMatchV5MatchTimelineInfoParticipants],
+        "endOfGameResult": str
     })
     LolMatchV5MatchTimeline = TypedDict("LolMatchV5MatchTimeline", {
         "metadata": LolMatchV5MatchTimelineMetadata,
         "info": LolMatchV5MatchTimelineInfo
     })
     LolSpectatorV4GameParticipantPerks = TypedDict("LolSpectatorV4GameParticipantPerks", {
         "perkIds": list[int],
@@ -1186,15 +1202,15 @@
         "puuid": str,
         "summonerId": str,
         "teamId": int,
         "spell1Id": int,
         "spell2Id": int,
         "championId": int,
         "profileIconId": int,
-        "summonerName": str,
+        "summonerName": NotRequired[str],
         "bot": bool
     })
     LolSpectatorV4GameObservers = TypedDict("LolSpectatorV4GameObservers", {
         "encryptionKey": str
     })
     LolSpectatorV4Game = TypedDict("LolSpectatorV4Game", {
         "gameId": int,
@@ -1209,43 +1225,72 @@
         "gameStartTime": int,
         "gameLength": int
     })
     LolSpectatorV4GameList = TypedDict("LolSpectatorV4GameList", {
         "gameList": list[LolSpectatorV4Game],
         "clientRefreshInterval": int
     })
+    LolSpectatorV5GameParticipant = TypedDict("LolSpectatorV5GameParticipant", {
+        "gameCustomizationObjects": NotRequired[list[str]],
+        "perks": NotRequired[LolSpectatorV4GameParticipantPerks],
+        "puuid": str,
+        "summonerId": str,
+        "teamId": int,
+        "spell1Id": int,
+        "spell2Id": int,
+        "championId": int,
+        "profileIconId": int,
+        "riotId": str,
+        "bot": bool,
+    })
+    LolSpectatorV5Game = TypedDict("LolSpectatorV5Game", {
+        "gameId": int,
+        "mapId": int,
+        "gameMode": str,
+        "gameType": str,
+        "gameQueueConfigId": int,
+        "participants": list[LolSpectatorV5GameParticipant],
+        "observers": LolSpectatorV4GameObservers,
+        "platformId": str,
+        "bannedChampions": list[int],
+        "gameStartTime": NotRequired[int],
+        "gameLength": int
+    })
+    LolSpectatorV5GameList = TypedDict("LolSpectatorV5GameList", {
+        "gameList": list[LolSpectatorV5Game],
+    })
     LolSummonerV4Summoner = TypedDict("SummonerV4Summoner", {
         "id": str,
         "accountId": str,
         "puuid": str,
-        "name": str,
+        "name": NotRequired[str],
         "profileIconId": int,
         "revisionDate": int,
         "summonerLevel": int
     })
 
     # Teamfight Tactics Types
 
     TftLeagueV1LeagueEntry = TypedDict("TftLeagueV1LeagueEntry", {
         "summonerId": str,
-        "summonerName": str,
+        "summonerName": NotRequired[str],
         "rank": str,
         "leaguePoints": int,
         "wins": int,
         "losses": int,
         "hotStreak": bool,
         "veteran": bool,
         "freshBlood": bool,
         "inactive": bool,
     })
     TftLeagueV1LeagueFullEntry = TypedDict("TftLeagueV1LeagueFullEntry", {
         "leagueId": str,
         "puuid": str,
         "summonerId": str,
-        "summonerName": str,
+        "summonerName": NotRequired[str],
         "queueType": str,
         "tier": str,
         "rank": str,
         "leaguePoints": int,
         "wins": int,
         "losses": int,
         "hotStreak": bool,
```

### Comparing `pulsefire-types-2.0.8/pulsefire_types.egg-info/PKG-INFO` & `pulsefire-types-2.0.9/pulsefire_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsefire-types
-Version: 2.0.8
+Version: 2.0.9
 Summary: A modern and flexible Riot Games Python SDK.
 Home-page: https://github.com/iann838/pulsefire
 Author: Jian Huang
 Author-email: iann838dev@gmail.com
 License: MIT
 Keywords: Riot Games,League of Legends,Teamfight Tactics,Valorant,Legends of Runeterra,API,SDK,asyncio
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pulsefire-types-2.0.8/setup.py` & `pulsefire-types-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Require python 3.7
 if sys.version_info < (3, 12):
     sys.exit("'pulsefire' requires Python >= 3.12")
 
 setup(
     name="pulsefire-types",
-    version="2.0.8",
+    version="2.0.9",
     author="Jian Huang",
     author_email="iann838dev@gmail.com",
     url="https://github.com/iann838/pulsefire",
     description="A modern and flexible Riot Games Python SDK.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Riot Games", "League of Legends", "Teamfight Tactics", "Valorant", "Legends of Runeterra", "API", "SDK", "asyncio"],
```

### Comparing `pulsefire-types-2.0.8/tests/test_base.py` & `pulsefire-types-2.0.9/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pulsefire-types-2.0.8/tests/test_caches.py` & `pulsefire-types-2.0.9/tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `pulsefire-types-2.0.8/tests/test_clients.py` & `pulsefire-types-2.0.9/tests/test_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,20 +107,20 @@
         await client.get_lol_league_v4_grandmaster_league_by_queue(region="na1", queue="RANKED_SOLO_5x5")
         await client.get_lol_league_v4_master_league_by_queue(region="na1", queue="RANKED_SOLO_5x5")
         await client.get_lol_league_v4_entries_by_division(region="na1", queue="RANKED_SOLO_5x5", tier="EMERALD", division="III", queries={"page": 10})
         match_ids = await client.get_lol_match_v5_match_ids_by_puuid(region="americas", puuid=summoner["puuid"])
         print(match_ids[0])
         await client.get_lol_match_v5_match(region="americas", id=match_ids[0])
         await client.get_lol_match_v5_match_timeline(region="americas", id=match_ids[0])
-        featured_games = await client.get_lol_spectator_v4_featured_games(region="na1")
-        await client.get_lol_spectator_v4_active_game_by_summoner(region="na1", summoner_id=featured_games["gameList"][0]["participants"][0]["summonerId"])
+        featured_games = await client.get_lol_spectator_v5_featured_games(region="na1")
+        await client.get_lol_spectator_v5_active_game_by_summoner(region="na1", puuid=featured_games["gameList"][0]["participants"][0]["puuid"])
         await client.get_lol_status_v4_platform_data(region="na1")
         await client.get_lol_summoner_v4_by_id(region="na1", id=summoner["id"])
-        await client.get_lol_summoner_v4_by_name(region="na1", name=summoner["name"])
-        await client.get_lol_summoner_v4_by_puuid(region="na1", puuid=summoner["puuid"])
+        # await client.get_lol_summoner_v4_by_name(region="na1", name=summoner["name"])
+        # await client.get_lol_summoner_v4_by_puuid(region="na1", puuid=summoner["puuid"])
 
 
 @async_to_sync()
 async def test_tft_riot_api_client():
     async with RiotAPIClient(default_headers={"X-Riot-Token": os.environ["TFT_API_KEY"]}) as client:
         plat_league = await client.get_tft_league_v1_entries_by_division(region="na1", tier="PLATINUM", division="II")
         summoner = await client.get_tft_summoner_v1_by_id(region="na1", id=plat_league[0]["summonerId"])
```

### Comparing `pulsefire-types-2.0.8/tests/test_doc_scripts.py` & `pulsefire-types-2.0.9/tests/test_doc_scripts.py`

 * *Files identical despite different names*

### Comparing `pulsefire-types-2.0.8/tests/test_ratelimiters.py` & `pulsefire-types-2.0.9/tests/test_ratelimiters.py`

 * *Files identical despite different names*

### Comparing `pulsefire-types-2.0.8/tests/test_taskgroups.py` & `pulsefire-types-2.0.9/tests/test_taskgroups.py`

 * *Files identical despite different names*

