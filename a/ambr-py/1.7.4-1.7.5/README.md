# Comparing `tmp/ambr_py-1.7.4.tar.gz` & `tmp/ambr_py-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambr_py-1.7.4.tar", max compression
+gzip compressed data, was "ambr_py-1.7.5.tar", max compression
```

## Comparing `ambr_py-1.7.4.tar` & `ambr_py-1.7.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       73 2023-12-02 07:02:04.398062 ambr_py-1.7.4/ambr/__init__.py
--rw-r--r--   0        0        0    19466 2024-03-27 06:08:39.164157 ambr_py-1.7.4/ambr/client.py
--rw-r--r--   0        0        0      660 2024-03-27 06:07:14.220344 ambr_py-1.7.4/ambr/exceptions.py
--rw-r--r--   0        0        0      415 2024-03-27 06:07:14.221339 ambr_py-1.7.4/ambr/models/__init__.py
--rw-r--r--   0        0        0     6960 2024-04-30 13:19:56.977337 ambr_py-1.7.4/ambr/models/abyss.py
--rw-r--r--   0        0        0     2855 2024-03-27 06:07:14.221339 ambr_py-1.7.4/ambr/models/achievement.py
--rw-r--r--   0        0        0     3796 2024-03-27 06:07:14.222234 ambr_py-1.7.4/ambr/models/artifact.py
--rw-r--r--   0        0        0     1871 2024-03-27 06:07:14.223233 ambr_py-1.7.4/ambr/models/book.py
--rw-r--r--   0        0        0      820 2024-03-27 06:07:14.223233 ambr_py-1.7.4/ambr/models/changelog.py
--rw-r--r--   0        0        0     8659 2024-03-27 06:07:14.224245 ambr_py-1.7.4/ambr/models/character.py
--rw-r--r--   0        0        0     2590 2024-03-27 06:07:14.225232 ambr_py-1.7.4/ambr/models/character_fetter.py
--rw-r--r--   0        0        0     1299 2024-03-27 06:07:14.225232 ambr_py-1.7.4/ambr/models/domain.py
--rw-r--r--   0        0        0     2994 2024-03-27 06:07:14.226269 ambr_py-1.7.4/ambr/models/food.py
--rw-r--r--   0        0        0     4548 2024-03-27 06:07:14.226269 ambr_py-1.7.4/ambr/models/furniture.py
--rw-r--r--   0        0        0     3047 2024-03-27 06:07:14.227232 ambr_py-1.7.4/ambr/models/material.py
--rw-r--r--   0        0        0     2420 2024-03-27 06:07:14.227232 ambr_py-1.7.4/ambr/models/monster.py
--rw-r--r--   0        0        0     1683 2024-03-27 06:07:14.228274 ambr_py-1.7.4/ambr/models/name_card.py
--rw-r--r--   0        0        0     1221 2024-03-27 06:07:14.228274 ambr_py-1.7.4/ambr/models/quest.py
--rw-r--r--   0        0        0     5209 2024-03-27 06:07:14.228274 ambr_py-1.7.4/ambr/models/tcg.py
--rw-r--r--   0        0        0      996 2024-03-27 06:07:14.229322 ambr_py-1.7.4/ambr/models/upgrade.py
--rw-r--r--   0        0        0     4267 2024-03-27 06:07:14.229322 ambr_py-1.7.4/ambr/models/weapon.py
--rw-r--r--   0        0        0     1117 2024-03-27 06:07:14.230244 ambr_py-1.7.4/ambr/utils.py
--rw-r--r--   0        0        0    35802 2023-06-22 15:33:58.568670 ambr_py-1.7.4/LICENSE
--rw-r--r--   0        0        0     1325 2024-05-14 02:58:12.851175 ambr_py-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     2302 2024-05-14 02:40:56.098319 ambr_py-1.7.4/README.md
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 ambr_py-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0       73 2024-01-15 00:08:53.036511 ambr_py-1.7.5/ambr/__init__.py
+-rw-r--r--   0        0        0    19669 2024-05-25 05:26:05.892430 ambr_py-1.7.5/ambr/client.py
+-rw-r--r--   0        0        0      660 2024-05-21 23:25:02.918034 ambr_py-1.7.5/ambr/exceptions.py
+-rw-r--r--   0        0        0      415 2024-02-25 01:39:24.545071 ambr_py-1.7.5/ambr/models/__init__.py
+-rw-r--r--   0        0        0     6940 2024-05-21 23:25:02.918034 ambr_py-1.7.5/ambr/models/abyss.py
+-rw-r--r--   0        0        0     2615 2024-05-21 23:25:02.918034 ambr_py-1.7.5/ambr/models/achievement.py
+-rw-r--r--   0        0        0     3494 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/artifact.py
+-rw-r--r--   0        0        0     1658 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/book.py
+-rw-r--r--   0        0        0      820 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/changelog.py
+-rw-r--r--   0        0        0     8659 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/character.py
+-rw-r--r--   0        0        0     2590 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/character_fetter.py
+-rw-r--r--   0        0        0     1299 2024-03-13 06:39:04.183353 ambr_py-1.7.5/ambr/models/domain.py
+-rw-r--r--   0        0        0     2994 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/food.py
+-rw-r--r--   0        0        0     5057 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/furniture.py
+-rw-r--r--   0        0        0     3050 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/material.py
+-rw-r--r--   0        0        0     2406 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/monster.py
+-rw-r--r--   0        0        0     1683 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/name_card.py
+-rw-r--r--   0        0        0     1221 2024-02-25 01:37:40.383910 ambr_py-1.7.5/ambr/models/quest.py
+-rw-r--r--   0        0        0     5209 2024-05-21 23:25:02.920478 ambr_py-1.7.5/ambr/models/tcg.py
+-rw-r--r--   0        0        0      996 2024-05-21 23:25:02.920478 ambr_py-1.7.5/ambr/models/upgrade.py
+-rw-r--r--   0        0        0     4270 2024-05-21 23:25:02.920478 ambr_py-1.7.5/ambr/models/weapon.py
+-rw-r--r--   0        0        0     1117 2024-02-25 01:37:40.384914 ambr_py-1.7.5/ambr/utils.py
+-rw-r--r--   0        0        0    35803 2024-01-15 00:08:53.036002 ambr_py-1.7.5/LICENSE
+-rw-r--r--   0        0        0     1625 2024-05-25 08:10:47.567573 ambr_py-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     2097 2024-05-15 01:10:41.857221 ambr_py-1.7.5/README.md
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 ambr_py-1.7.5/PKG-INFO
```

### Comparing `ambr_py-1.7.4/ambr/client.py` & `ambr_py-1.7.5/ambr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import logging
 from enum import Enum
-from typing import Any, Final
+from typing import TYPE_CHECKING, Any, Final, Self
 
 from aiohttp_client_cache.backends.sqlite import SQLiteBackend
 from aiohttp_client_cache.session import CachedSession
 
 from .exceptions import AmbrAPIError, ConnectionTimeoutError, DataNotFoundError
 from .models import (
     AbyssResponse,
@@ -34,14 +36,17 @@
     UpgradeData,
     Weapon,
     WeaponDetail,
 )
 from .models.furniture import FurnitureSet, FurnitureSetDetail
 from .utils import remove_html_tags
 
+if TYPE_CHECKING:
+    import aiohttp
+
 __all__ = ("AmbrAPI", "Language")
 
 
 class Language(Enum):
     CHT = "cht"
     CHS = "chs"
     DE = "de"
@@ -67,23 +72,23 @@
 
     def __init__(
         self,
         *,
         lang: Language = Language.EN,
         cache_ttl: int = 3600,
         headers: dict[str, Any] | None = None,
+        session: aiohttp.ClientSession | None = None,
     ) -> None:
         self.lang = lang
-        self.cache_ttl = cache_ttl
+        self._cache_ttl = cache_ttl
 
-        self._session: CachedSession | None = None
-        self._cache = SQLiteBackend("./.cache/ambr/aiohttp-cache.db", expire_after=cache_ttl)
+        self._session = session
         self._headers = headers or {"User-Agent": "ambr-py"}
 
-    async def __aenter__(self) -> "AmbrAPI":
+    async def __aenter__(self) -> Self:
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb) -> None:  # noqa: ANN001
         await self.close()
 
     async def _request(
@@ -113,15 +118,15 @@
         if static:
             url = f"{self.BASE_URL}/static/{endpoint}"
         else:
             url = f"{self.BASE_URL}/{self.lang.value}/{endpoint}"
 
         LOGGER_.debug("Requesting %s...", url)
 
-        if not use_cache:
+        if not use_cache and isinstance(self._session, CachedSession):
             async with self._session.disabled(), self._session.get(url) as resp:
                 if resp.status != 200:
                     self._handle_error(resp.status)
                 data = await resp.json()
         else:
             async with self._session.get(url) as resp:
                 if resp.status != 200:
@@ -142,15 +147,18 @@
             case _:
                 raise AmbrAPIError(code)
 
     async def start(self) -> None:
         """
         Starts the client session.
         """
-        self._session = CachedSession(headers=self._headers, cache=self._cache)
+        self._session = self._session or CachedSession(
+            headers=self._headers,
+            cache=SQLiteBackend("./.cache/ambr/aiohttp-cache.db", expire_after=self._cache_ttl),
+        )
 
     async def close(self) -> None:
         """
         Closes the client session.
         """
         if self._session is not None:
             await self._session.close()
```

### Comparing `ambr_py-1.7.4/ambr/exceptions.py` & `ambr_py-1.7.5/ambr/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ("AmbrAPIError", "DataNotFoundError", "ConnectionTimeoutError")
+__all__ = ("AmbrAPIError", "ConnectionTimeoutError", "DataNotFoundError")
 
 
 class AmbrAPIError(Exception):
     def __init__(self, code: int) -> None:
         self.code = code
 
     def __str__(self) -> str:
```

### Comparing `ambr_py-1.7.4/ambr/models/abyss.py` & `ambr_py-1.7.5/ambr/models/abyss.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
-    "ChallengeTarget",
-    "Chamber",
-    "LeyLineDisorder",
-    "Floor",
-    "AbyssData",
     "Abyss",
+    "AbyssData",
     "AbyssEnemy",
     "AbyssResponse",
     "Blessing",
+    "ChallengeTarget",
+    "Chamber",
+    "Floor",
+    "LeyLineDisorder",
 )
 
 
 class Blessing(BaseModel):
     """
     Blessing model.
 
@@ -39,15 +39,15 @@
 
 class ChallengeTarget(BaseModel):
     """
     ChallengeTarget model.
 
     Attributes:
         type (str): Type of the challenge target.
-        values (List[int]): List of values.
+        values (list[int]): list of values.
         formatted (str): Formatted challenge target.
     """
 
     type: str
     values: list[int]
 
     @property
@@ -59,16 +59,16 @@
     """
     Chamber model.
 
     Attributes:
         id (int): ID of the chamber.
         challenge_target (ChallengeTarget): Challenge target.
         enemy_level (int): Enemy level.
-        wave_one_enemies (List[int]): List of enemies in the first wave.
-        wave_two_enemies (Optional[List[int]]): List of enemies in the second wave.
+        wave_one_enemies (list[int]): list of enemies in the first wave.
+        wave_two_enemies (list[int] | None): list of enemies in the second wave.
     """
 
     id: int
     challenge_target: ChallengeTarget = Field(..., alias="challengeTarget")
     enemy_level: int = Field(..., alias="monsterLevel")
     wave_one_enemies: list[int] = Field(..., alias="firstMonsterList")
     wave_two_enemies: list[int] | None = Field(None, alias="secondMonsterList")
@@ -95,16 +95,16 @@
 
 class Floor(BaseModel):
     """
     Floor model.
 
     Attributes:
         id (int): ID of the floor.
-        chambers (List[Chamber]): List of chambers.
-        ley_line_disorders (List[LeyLineDisorder]): List of ley line disorders.
+        chambers (list[Chamber]): list of chambers.
+        ley_line_disorders (list[LeyLineDisorder]): list of ley line disorders.
         override_enemy_level (int): Override enemy level.
         team_num (int): Number of teams.
     """
 
     id: int
     chambers: list[Chamber] = Field(..., alias="chamberList")
     ley_line_disorders: list[LeyLineDisorder] = Field(..., alias="leyLineDisorder")
@@ -113,16 +113,16 @@
 
 
 class AbyssData(BaseModel):
     """
     AbyssData model.
 
     Attributes:
-        open_time (Optional[datetime.datetime]): Opening time.
-        floors (List[Floor]): List of floors.
+        open_time (datetime.datetime | None): Opening time.
+        floors (list[Floor]): list of floors.
     """
 
     open_time: datetime.datetime | None = Field(None, alias="openTime")
     floors: list[Floor] = Field(..., alias="floorList")
 
     @field_validator("open_time", mode="before")
     def _format_open_time(cls, v: int) -> datetime.datetime | None:
@@ -194,28 +194,28 @@
     id: int
     link: bool
     name: str
     properties: list[AbyssEnemyProperty] = Field(..., alias="prop")
 
     @field_validator("icon", mode="before")
     def _convert_icon_url(cls, v: str) -> str:
-        return f"https://api.ambr.top/assets/UI{'/monster' if 'MonsterIcon' in v else ''}/{v}.png"  # noqa: E501
+        return f"https://api.ambr.top/assets/UI{'/monster' if 'MonsterIcon' in v else ''}/{v}.png"
 
     @field_validator("properties", mode="before")
     def _convert_properties(cls, v: list[dict[str, Any]]) -> list[AbyssEnemyProperty]:
         return [AbyssEnemyProperty(**prop) for prop in v]
 
 
 class AbyssResponse(BaseModel):
     """
     AbyssResponse model.
 
     Attributes:
-        enemies (Dict[str, AbyssEnemy]): Dictionary of abyss enemies.
-        abyss_items (List[Abyss]): List of abyss items.
+        enemies (dict[str, AbyssEnemy]): Dictionary of abyss enemies.
+        abyss_items (list[Abyss]): list of abyss items.
     """
 
     enemies: dict[str, AbyssEnemy] = Field(..., alias="monsterList")
     abyss_items: list[Abyss] = Field(..., alias="items")
 
     @field_validator("enemies", mode="before")
     def _convert_enemies(cls, v: dict[str, dict[str, Any]]) -> dict[str, AbyssEnemy]:
```

### Comparing `ambr_py-1.7.4/ambr/models/achievement.py` & `ambr_py-1.7.5/ambr/models/achievement.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 __all__ = (
-    "AchievementReward",
-    "AchievementDetail",
     "Achievement",
     "AchievementCategory",
+    "AchievementDetail",
+    "AchievementReward",
 )
 
 
 class AchievementReward(BaseModel):
     """
     Represents an achievement reward.
 
-    Attributes
-    ----------
-    rarity: :class:`int`
-        The achievement reward's rarity.
-    amount: :class:`int`
-        The achievement reward's amount.
-    icon: :class:`str`
-        The achievement reward's icon.
+    Attributes:
+        rarity (int): The achievement reward's rarity.
+        amount (int): The achievement reward's amount.
+        icon (str): The achievement reward's icon.
     """
 
     rarity: int = Field(alias="rank")
     amount: int = Field(alias="count")
     icon: str
 
     @field_validator("icon", mode="before")
@@ -33,24 +29,19 @@
         return f"https://api.ambr.top/assets/UI/{v}.png"
 
 
 class AchievementDetail(BaseModel):
     """
     Represents an achievement detail.
 
-    Attributes
-    ----------
-    id: :class:`int`
-        The achievement's ID.
-    title: :class:`str`
-        The achievement's title.
-    description: :class:`str`
-        The achievement's description.
-    rewards: List[:class:`AchievementReward`]
-        The achievement's rewards.
+    Attributes:
+        id (int): The achievement's ID.
+        title (str): The achievement's title.
+        description (str): The achievement's description.
+        rewards (list[AchievementReward]): The achievement's rewards.
     """
 
     id: int
     title: str
     description: str
     rewards: list[AchievementReward]
 
@@ -59,45 +50,35 @@
         return [AchievementReward(**v[item_id]) for item_id in v]
 
 
 class Achievement(BaseModel):
     """
     Represents an achievement.
 
-    Attributes
-    ----------
-    id: :class:`int`
-        The achievement's ID.
-    order: :class:`int`
-        The achievement's order.
-    details: List[:class:`AchievementDetail`]
-        The achievement's details.
+    Attributes:
+        id (int): The achievement's ID.
+        order (int): The achievement's order.
+        details (list[AchievementDetail]): The achievement's details.
     """
 
     id: int
     order: int
     details: list[AchievementDetail]
 
 
 class AchievementCategory(BaseModel):
     """
     Represents an achievement category.
 
-    Attributes
-    ----------
-    id: :class:`int`
-        The achievement category's ID.
-    name: :class:`str`
-        The achievement category's name.
-    order: :class:`int`
-        The achievement category's order.
-    icon: :class:`str`
-        The achievement category's icon.
-    achievements: List[:class:`Achievement`]
-        The achievement category's achievements.
+    Attributes:
+        id (int): The achievement category's ID.
+        name (str): The achievement category's name.
+        order (int): The achievement category's order.
+        icon (str): The achievement category's icon.
+        achievements (list[Achievement]): The achievement category's achievements.
     """
 
     id: int
     name: str
     order: int
     icon: str
     achievements: list[Achievement] = Field(alias="achievementList")
```

### Comparing `ambr_py-1.7.4/ambr/models/artifact.py` & `ambr_py-1.7.5/ambr/models/artifact.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 __all__ = (
-    "ArtifactAffix",
     "Artifact",
-    "ArtifactSetDetail",
+    "ArtifactAffix",
     "ArtifactSet",
+    "ArtifactSetDetail",
 )
 
 
 class ArtifactAffix(BaseModel):
     """
     Represents an artifact set's set effect.
 
-    Attributes
-    ----------
-    id: :class:`str`
-        The effect's ID.
-    effect: :class:`str`
-        The effect's description.
+    Attributes:
+        id (str): The effect's ID.
+        effect (str): The effect's description.
     """
 
     id: str
     effect: str
 
 
 class Artifact(BaseModel):
     """
     Represents an artifact.
 
-    Attributes
-    ----------
-    pos: :class:`str`
-        The position of the artifact.
-    name: :class:`str`
-        The name of the artifact.
-    description: :class:`str`
-        The description of the artifact.
-    max_rarity: :class:`int`
-        The maximum rarity of the artifact.
-    icon: :class:`str`
-        The name of the icon file for the artifact.
+    Attributes:
+        pos (str): The position of the artifact.
+        name (str): The name of the artifact.
+        description (str): The description of the artifact.
+        max_rarity (int): The maximum rarity of the artifact.
+        icon (str): The name of the icon file for the artifact.
     """
 
     pos: str
     name: str
     description: str
     max_rarity: int = Field(alias="maxLevel")
     icon: str
@@ -55,30 +46,22 @@
         return f"https://api.ambr.top/assets/UI/reliquary/{v}.png"
 
 
 class ArtifactSetDetail(BaseModel):
     """
     Represents an artifact set detail.
 
-    Attributes
-    ----------
-    id: :class:`int`
-        The artifact set's ID.
-    name: :class:`str`
-        The artifact set's name.
-    rarity_list: List[:class:`int`]
-        The artifact set's rarity list.
-    affix_list: List[:class:`ArtifactAffix`]
-        The artifact set's affix list.
-    icon: :class:`str`
-        The artifact set's icon.
-    route: :class:`str`
-        The artifact set's route.
-    artifacts: List[:class:`Artifact`]
-        Artifacts that belong to the artifact set.
+    Attributes:
+        id (int): The artifact set's ID.
+        name (str): The artifact set's name.
+        rarity_list (list[int]): The artifact set's rarity list.
+        affix_list (list[ArtifactAffix]): The artifact set's affix list.
+        icon (str): The artifact set's icon.
+        route (str): The artifact set's route.
+        artifacts (list[Artifact]): Artifacts that belong to the artifact set.
     """
 
     id: int
     name: str
     rarity_list: list[int] = Field(alias="levelList")
     affix_list: list[ArtifactAffix] = Field(alias="affixList")
     icon: str
@@ -98,30 +81,22 @@
         return [Artifact(pos=artifact_pos, **v[artifact_pos]) for artifact_pos in v]
 
 
 class ArtifactSet(BaseModel):
     """
     Represents an artifact set.
 
-    Attributes
-    ----------
-    id: :class:`int`
-        The artifact set's ID.
-    name: :class:`str`
-        The artifact set's name.
-    rarity_list: List[:class:`int`]
-        Obtainable rarities of the artifact set.
-    affix_list: List[:class:`str`]
-        The artifact set's set effect list.
-    icon: :class:`str`
-        The artifact set's icon.
-    route: :class:`str`
-        The artifact set's route.
-    sort_order: :class:`int`
-        The artifact set's sort order.
+    Attributes:
+        id (int): The artifact set's ID.
+        name (str): The artifact set's name.
+        rarity_list (list[int]): Obtainable rarities of the artifact set.
+        affix_list (list[ArtifactAffix]): The artifact set's set effect list.
+        icon (str): The artifact set's icon.
+        route (str): The artifact set's route.
+        sort_order (int): The artifact set's sort order.
     """
 
     id: int
     name: str
     rarity_list: list[int] = Field(alias="levelList")
     affix_list: list[ArtifactAffix] = Field(alias="affixList")
     icon: str
```

### Comparing `ambr_py-1.7.4/ambr/models/changelog.py` & `ambr_py-1.7.5/ambr/models/changelog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import BaseModel, Field, field_validator
 
 __all__ = (
-    "Item",
     "Changelog",
+    "Item",
 )
 
 
 class Item(BaseModel):
     category: str
     ids: list[str]
```

### Comparing `ambr_py-1.7.4/ambr/models/character.py` & `ambr_py-1.7.5/ambr/models/character.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
-    "Element",
+    "AscensionMaterial",
     "Birthday",
+    "Character",
+    "CharacterBaseStat",
+    "CharacterCV",
+    "CharacterDetail",
+    "CharacterInfo",
+    "CharacterPromote",
+    "CharacterPromoteMaterial",
+    "CharacterPromoteStat",
+    "CharacterUpgrade",
+    "Constellation",
+    "Element",
     "ExtraLevelType",
+    "Talent",
     "TalentExtraLevel",
-    "Constellation",
     "TalentType",
-    "TalentUpgradeItem",
     "TalentUpgrade",
-    "Talent",
-    "AscensionMaterial",
-    "CharacterPromoteStat",
-    "CharacterPromoteMaterial",
-    "CharacterPromote",
-    "CharacterBaseStat",
-    "CharacterUpgrade",
-    "CharacterCV",
-    "CharacterInfo",
-    "CharacterDetail",
-    "Character",
+    "TalentUpgradeItem",
 )
 
 
 class Element(StrEnum):
     ANEMO = "Wind"
     GEO = "Rock"
     ELECTRO = "Electric"
```

### Comparing `ambr_py-1.7.4/ambr/models/character_fetter.py` & `ambr_py-1.7.5/ambr/models/character_fetter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags, replace_pronouns
 
-__all__ = ("Quest", "Task", "Quote", "Story", "CharacterFetter")
+__all__ = ("CharacterFetter", "Quest", "Quote", "Story", "Task")
 
 
 class Quest(BaseModel):
     id: int
     quest_title: str | None = Field(None, alias="questTitle")
     chapter_id: int = Field(alias="chapterId")
     chapter_title: str = Field(alias="chapterTitle")
```

### Comparing `ambr_py-1.7.4/ambr/models/domain.py` & `ambr_py-1.7.5/ambr/models/domain.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.4/ambr/models/food.py` & `ambr_py-1.7.5/ambr/models/food.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
-    "FoodSource",
+    "Food",
+    "FoodDetail",
     "FoodEffect",
     "FoodRecipe",
-    "FoodDetail",
-    "Food",
+    "FoodSource",
 )
 
 
 class FoodSource(BaseModel):
     name: str
     type: str
```

### Comparing `ambr_py-1.7.4/ambr/models/furniture.py` & `ambr_py-1.7.5/ambr/models/furniture.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
-    "FurnitureRecipeInput",
-    "FurnitureRecipe",
-    "FurnitureDetail",
     "Furniture",
-    "FurnitureSet",
+    "FurnitureDetail",
     "FurnitureItem",
+    "FurnitureRecipe",
+    "FurnitureRecipeInput",
+    "FurnitureSet",
     "FurnitureSetDetail",
 )
 
 
 class FurnitureRecipeInput(BaseModel):
     id: int
     icon: str
@@ -127,23 +127,29 @@
     icon: str
 
     @field_validator("icon", mode="before")
     def _convert_icon_url(cls, v: str) -> str:
         return f"https://api.ambr.top/assets/UI/furniture/{v}.png"
 
 
+class FurnitureSetFavoriteNPC(BaseModel):
+    id: str
+    icon: str
+
+
 class FurnitureSetDetail(BaseModel):
     id: int
     name: str
     icon: str
     route: str
     categories: list[str]
     types: list[str]
     description: str
     furniture_items: list[FurnitureItem] = Field(alias="suiteItemList")
+    favorite_npcs: list[FurnitureSetFavoriteNPC] = Field(alias="favoriteNpcList")
 
     @field_validator("icon", mode="before")
     def _convert_icon_url(cls, v: str) -> str:
         return f"https://api.ambr.top/assets/UI/furnitureSuite/{v}.png"
 
     @field_validator("categories", mode="before")
     def _convert_categories(cls, v: list[str] | None) -> list[str]:
@@ -156,7 +162,17 @@
     @field_validator("description", mode="before")
     def _format_description(cls, v: str) -> str:
         return remove_html_tags(v)
 
     @field_validator("furniture_items", mode="before")
     def _convert_furniture_items(cls, v: dict[str, dict[str, Any]]) -> list[FurnitureItem]:
         return [FurnitureItem(id=int(item_id), **v[item_id]) for item_id in v]
+
+    @field_validator("favorite_npcs", mode="before")
+    def _convert_favored_ids(
+        cls, v: dict[str, dict[str, Any]] | None
+    ) -> list[FurnitureSetFavoriteNPC]:
+        return (
+            [FurnitureSetFavoriteNPC(id=id_, icon=data["icon"]) for id_, data in v.items()]
+            if v is not None
+            else []
+        )
```

### Comparing `ambr_py-1.7.4/ambr/models/material.py` & `ambr_py-1.7.5/ambr/models/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
+    "Material",
+    "MaterialDetail",
     "MaterialRecipe",
     "MaterialSource",
-    "MaterialDetail",
-    "Material",
 )
 
 WEEKDAYS = {
     "monday": 1,
     "tuesday": 2,
     "wednesday": 3,
     "thursday": 4,
@@ -57,15 +57,15 @@
         return remove_html_tags(v)
 
     @field_validator("recipe", mode="before")
     def _convert_recipe(
         cls, v: bool | dict[str, dict[str, dict[str, Any]]]
     ) -> list[MaterialRecipe]:
         if isinstance(v, dict):
-            recipe = list(v.values())[0]
+            recipe = next(iter(v.values()))
             return [MaterialRecipe(**item) for item in recipe.values()]
         return []
 
     @field_validator("sources", mode="before")
     def _convert_sources(cls, v: list[dict] | None) -> list[MaterialSource]:
         return [MaterialSource(**item) for item in v] if v else []
```

### Comparing `ambr_py-1.7.4/ambr/models/monster.py` & `ambr_py-1.7.5/ambr/models/monster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
-    "MonsterReward",
-    "MonsterEntry",
-    "MonsterDetail",
     "Monster",
+    "MonsterDetail",
+    "MonsterEntry",
+    "MonsterReward",
 )
 
 
 class MonsterReward(BaseModel):
     id: int
     rarity: int = Field(alias="rank")
     icon: str
@@ -42,15 +42,15 @@
     title: str | None
     special_name: str | None = Field(alias="specialName")
     description: str
     entries: list[MonsterEntry]
 
     @field_validator("icon", mode="before")
     def _convert_icon_url(cls, v: str) -> str:
-        return f"https://api.ambr.top/assets/UI{'/monster' if 'MonsterIcon' in v else ''}/{v}.png"  # noqa: E501
+        return f"https://api.ambr.top/assets/UI{'/monster' if 'MonsterIcon' in v else ''}/{v}.png"
 
     @field_validator("entries", mode="before")
     def _convert_entries(cls, v: dict[str, dict[str, Any]]) -> list[MonsterEntry]:
         return [MonsterEntry(**v[item_id]) for item_id in v]
 
     @field_validator("description", mode="before")
     def _format_description(cls, v: str) -> str:
```

### Comparing `ambr_py-1.7.4/ambr/models/name_card.py` & `ambr_py-1.7.5/ambr/models/name_card.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
-    "NamecardDetail",
     "Namecard",
+    "NamecardDetail",
 )
 
 
 class NamecardDetail(BaseModel):
     id: int
     name: str
     rarity: int = Field(alias="rank")
```

### Comparing `ambr_py-1.7.4/ambr/models/quest.py` & `ambr_py-1.7.5/ambr/models/quest.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.4/ambr/models/tcg.py` & `ambr_py-1.7.5/ambr/models/tcg.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags, replace_placeholders
 
 __all__ = (
-    "CardTag",
-    "DiceCost",
     "CardDictionary",
+    "CardTag",
     "CardTalent",
-    "TCGCardDetail",
+    "DiceCost",
     "TCGCard",
+    "TCGCardDetail",
 )
 
 
 class CardTag(BaseModel):
     id: str
     name: str
```

### Comparing `ambr_py-1.7.4/ambr/models/upgrade.py` & `ambr_py-1.7.5/ambr/models/upgrade.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 __all__ = (
-    "UpgradeItem",
     "Upgrade",
     "UpgradeData",
+    "UpgradeItem",
 )
 
 
 class UpgradeItem(BaseModel):
     id: int
     rarity: int
```

### Comparing `ambr_py-1.7.4/ambr/models/weapon.py` & `ambr_py-1.7.5/ambr/models/weapon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any
 
 from pydantic import BaseModel, Field, field_validator
 
 from ..utils import remove_html_tags
 
 __all__ = (
+    "Weapon",
+    "WeaponAffix",
+    "WeaponAffixUpgrade",
     "WeaponAscensionMaterial",
-    "WeaponPromoteCostItem",
-    "WeaponPromote",
     "WeaponBaseStat",
-    "WeaponUpgrade",
-    "WeaponAffixUpgrade",
-    "WeaponAffix",
     "WeaponDetail",
-    "Weapon",
+    "WeaponPromote",
+    "WeaponPromoteCostItem",
+    "WeaponUpgrade",
 )
 
 
 class WeaponAscensionMaterial(BaseModel):
     id: int
     rarity: int
 
@@ -100,15 +100,15 @@
     def _convert_icon_url(cls, v: str) -> str:
         return f"https://api.ambr.top/assets/UI/{v}.png"
 
     @field_validator("affix", mode="before")
     def _convert_affix(cls, v: dict[str, dict[str, Any]] | None) -> WeaponAffix | None:
         if v is None:
             return None
-        affix = list(v.values())[0]
+        affix = next(iter(v.values()))
         return WeaponAffix(**affix)
 
     @field_validator("ascension_materials", mode="before")
     def _convert_ascension_materials(cls, v: dict[str, int]) -> list[WeaponAscensionMaterial]:
         return [WeaponAscensionMaterial(id=int(k), rarity=v[k]) for k in v]
```

### Comparing `ambr_py-1.7.4/ambr/utils.py` & `ambr_py-1.7.5/ambr/utils.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.4/LICENSE` & `ambr_py-1.7.5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ambr_py-1.7.4/README.md` & `ambr_py-1.7.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 > Note: I am not the developer of Project Ambr.
 
 ### Features
 
 - Fully typed.
 - Fully asynchronous by using `aiofiles`, `aiohttp`, and `asyncio`, suitable for Discord bots.
 - Provides direct icon URLs.
-- Supports Python 3.10+.
+- Supports Python 3.11+.
 - Supports all game languages.
-- Supports both Genshin Impact and Honkai Star Rail.
 - Supports persistent caching using SQLite.
 - Supports [Pydantic V2](https://github.com/pydantic/pydantic), this also means full autocomplete support.
-- Seamlessly integrates with [GenshinData](https://gitlab.com/Dimbreath/AnimeGameData) and [StarRailData](https://github.com/Dimbreath/StarRailData).
 
 ## Installation
 
 ```bash
 # poetry
 poetry add ambr-py
```

### Comparing `ambr_py-1.7.4/PKG-INFO` & `ambr_py-1.7.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambr-py
-Version: 1.7.4
+Version: 1.7.5
 Summary: API wrapper for ambr.top written in Python
 License: GPL-3.0
 Author: seriaati
 Author-email: seria.ati@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -34,20 +34,18 @@
 > Note: I am not the developer of Project Ambr.
 
 ### Features
 
 - Fully typed.
 - Fully asynchronous by using `aiofiles`, `aiohttp`, and `asyncio`, suitable for Discord bots.
 - Provides direct icon URLs.
-- Supports Python 3.10+.
+- Supports Python 3.11+.
 - Supports all game languages.
-- Supports both Genshin Impact and Honkai Star Rail.
 - Supports persistent caching using SQLite.
 - Supports [Pydantic V2](https://github.com/pydantic/pydantic), this also means full autocomplete support.
-- Seamlessly integrates with [GenshinData](https://gitlab.com/Dimbreath/AnimeGameData) and [StarRailData](https://github.com/Dimbreath/StarRailData).
 
 ## Installation
 
 ```bash
 # poetry
 poetry add ambr-py
```

