# Comparing `tmp/sqlalchemy_celery_beat-0.4.2.tar.gz` & `tmp/sqlalchemy_celery_beat-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.4.2.tar", last modified: Thu Jun 15 10:08:31 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.4.4.tar", last modified: Thu Jun 15 17:41:11 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.4.2.tar` & `sqlalchemy_celery_beat-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 10:08:31.526233 sqlalchemy_celery_beat-0.4.2/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     9217 2023-06-15 10:08:31.525230 sqlalchemy_celery_beat-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     8273 2023-06-15 09:59:41.000000 sqlalchemy_celery_beat-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 10:08:31.526233 sqlalchemy_celery_beat-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2982 2023-06-15 10:08:04.000000 sqlalchemy_celery_beat-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 10:08:31.491232 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      239 2023-06-15 08:46:52.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0    10470 2023-06-15 09:27:41.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16331 2023-06-15 09:27:41.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     2088 2023-06-15 08:46:52.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1229 2023-06-15 09:06:15.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-15 10:08:31.522239 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0     9217 2023-06-15 10:08:31.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-15 10:08:31.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 10:08:31.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 09:31:58.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-15 10:08:31.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-15 10:08:31.000000 sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 17:41:11.110450 sqlalchemy_celery_beat-0.4.4/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     9410 2023-06-15 17:41:11.109451 sqlalchemy_celery_beat-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8462 2023-06-15 17:35:29.000000 sqlalchemy_celery_beat-0.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 17:41:11.110450 sqlalchemy_celery_beat-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     2982 2023-06-15 17:35:46.000000 sqlalchemy_celery_beat-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:41:11.078447 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      255 2023-06-15 17:39:21.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    13060 2023-06-15 17:22:39.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16954 2023-06-15 17:34:05.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     2272 2023-06-15 12:12:30.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:41:11.107449 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0     9410 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.4.2/LICENSE` & `sqlalchemy_celery_beat-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.2/PKG-INFO` & `sqlalchemy_celery_beat-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.4.2
+Version: 0.4.4
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -86,15 +86,18 @@
 from celery import Celery
 
 celery = Celery('tasks')
 
 beat_dburi = 'sqlite:///schedule.db'
 
 celery.conf.update(
-    {'beat_dburi': beat_dburi}
+    {
+        'beat_dburi': beat_dburi,
+        'beat_schema': None  # you can make the scheduler tables under different schema (tested for postgresql, not available in sqlite)
+    }
 )
 ```
 
 Also, you can use MySQL or PostgreSQL.
 
 ```Python
 # MySQL: `pip install mysql-connector`
@@ -266,17 +269,18 @@
 2.  As a separate process, start the beat service (specify the
     scheduler):
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## TO BE ADDED LATER
 
-- Add `ClockedSchedule` model
-- Tests
+- ✅ Add `ClockedSchedule` model
+- Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
+- Use Alembic migrations
 
 Any help is appreciated 🙂
 
 ## Acknowledgments
 
 - [django-celery-beat](https://github.com/celery/django-celery-beat)
 - [celerybeatredis](https://github.com/liuliqiang/celerybeatredis)
```

### Comparing `sqlalchemy_celery_beat-0.4.2/README.md` & `sqlalchemy_celery_beat-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,18 @@
 from celery import Celery
 
 celery = Celery('tasks')
 
 beat_dburi = 'sqlite:///schedule.db'
 
 celery.conf.update(
-    {'beat_dburi': beat_dburi}
+    {
+        'beat_dburi': beat_dburi,
+        'beat_schema': None  # you can make the scheduler tables under different schema (tested for postgresql, not available in sqlite)
+    }
 )
 ```
 
 Also, you can use MySQL or PostgreSQL.
 
 ```Python
 # MySQL: `pip install mysql-connector`
@@ -247,17 +250,18 @@
 2.  As a separate process, start the beat service (specify the
     scheduler):
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## TO BE ADDED LATER
 
-- Add `ClockedSchedule` model
-- Tests
+- ✅ Add `ClockedSchedule` model
+- Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
+- Use Alembic migrations
 
 Any help is appreciated 🙂
 
 ## Acknowledgments
 
 - [django-celery-beat](https://github.com/celery/django-celery-beat)
 - [celerybeatredis](https://github.com/liuliqiang/celerybeatredis)
```

### Comparing `sqlalchemy_celery_beat-0.4.2/setup.py` & `sqlalchemy_celery_beat-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.4.2",
+    version="0.4.4",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding=utf-8
 
 import datetime as dt
 from zoneinfo import ZoneInfo
 
 import sqlalchemy as sa
-from sqlalchemy import func
-from sqlalchemy.event import listen
-from sqlalchemy.orm import relationship, foreign, remote
-from sqlalchemy.sql import select, insert, update
-
 from celery import schedules
 from celery.utils.log import get_logger
+from sqlalchemy import func
+from sqlalchemy.event import listen, listens_for
+from sqlalchemy.orm import foreign, relationship, remote, validates
+from sqlalchemy.sql import insert, select, update
 
-from .tzcrontab import TzAwareCrontab
+from .clockedschedule import clocked
 from .session import ModelBase
-
+from .tzcrontab import TzAwareCrontab
 
 logger = get_logger('sqlalchemy_celery_beat.models')
 
 
 def cronexp(field):
     """Representation of cron expression."""
     return field and str(field).replace(' ', '') or '*'
@@ -34,15 +33,18 @@
         for attr, value in kw.items():
             setattr(self, attr, value)
         return self
 
 
 class IntervalSchedule(ModelBase, ModelMixin):
     __tablename__ = 'celery_interval_schedule'
-    __table_args__ = {'sqlite_autoincrement': True}
+    __table_args__ = {
+        'sqlite_autoincrement': True,
+        'schema': 'celery_schema'
+    }
 
     DAYS = 'days'
     HOURS = 'hours'
     MINUTES = 'minutes'
     SECONDS = 'seconds'
     MICROSECONDS = 'microseconds'
 
@@ -78,15 +80,18 @@
     @property
     def period_singular(self):
         return self.period[:-1]
 
 
 class CrontabSchedule(ModelBase, ModelMixin):
     __tablename__ = 'celery_crontab_schedule'
-    __table_args__ = {'sqlite_autoincrement': True}
+    __table_args__ = {
+        'sqlite_autoincrement': True,
+        'schema': 'celery_schema'
+    }
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
     minute = sa.Column(sa.String(60 * 4), default='*')
     hour = sa.Column(sa.String(24 * 4), default='*')
     day_of_week = sa.Column(sa.String(64), default='*')
     day_of_month = sa.Column(sa.String(31 * 4), default='*')
     month_of_year = sa.Column(sa.String(64), default='*')
@@ -116,27 +121,30 @@
             'hour': schedule._orig_hour,
             'day_of_week': schedule._orig_day_of_week,
             'day_of_month': schedule._orig_day_of_month,
             'month_of_year': schedule._orig_month_of_year,
         }
         if schedule.tz:
             spec.update({
-                'timezone': schedule.tz.zone
+                'timezone': schedule.tz.key
             })
         model = session.query(CrontabSchedule).filter_by(**spec).first()
         if not model:
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
 
 class SolarSchedule(ModelBase, ModelMixin):
     __tablename__ = 'celery_solar_schedule'
-    __table_args__ = {'sqlite_autoincrement': True}
+    __table_args__ = {
+        'sqlite_autoincrement': True,
+        'schema': 'celery_schema'
+    }
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
 
     event = sa.Column(sa.String(24))
     latitude = sa.Column(sa.Float())
     longitude = sa.Column(sa.Float())
 
@@ -167,18 +175,48 @@
         return '{0} ({1}, {2})'.format(
             self.event,
             self.latitude,
             self.longitude
         )
 
 
+class ClockedSchedule(ModelBase, ModelMixin):
+    __tablename__ = 'celery_clocked_schedule'
+    __table_args__ = {
+        'sqlite_autoincrement': True,
+        'schema': 'celery_schema'
+    }
+
+    id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
+    clocked_time = sa.Column(sa.DateTime(timezone=True))
+
+    def __repr__(self):
+        return f'{self.clocked_time}'
+
+    @property
+    def schedule(self):
+        c = clocked(clocked_time=self.clocked_time)
+        return c
+
+    @classmethod
+    def from_schedule(cls, session, schedule):
+        spec = {'clocked_time': schedule.clocked_time}
+        model = session.query(ClockedSchedule).filter_by(**spec).first()
+        if not model:
+            model = cls(**spec)
+            session.add(model)
+            session.commit()
+        return model
+
+
 class PeriodicTaskChanged(ModelBase, ModelMixin):
     """Helper table for tracking updates to periodic tasks."""
 
     __tablename__ = 'celery_periodic_task_changed'
+    __table_args__ = {'schema': 'celery_schema'}
 
     id = sa.Column(sa.Integer, primary_key=True)
     last_update = sa.Column(
         sa.DateTime(timezone=True), nullable=False, default=dt.datetime.now)
 
     @classmethod
     def changed(cls, mapper, connection, target):
@@ -193,15 +231,15 @@
     @classmethod
     def update_changed(cls, mapper, connection, target):
         """
         :param mapper: the Mapper which is the target of this event
         :param connection: the Connection being used
         :param target: the mapped instance being persisted
         """
-        s = connection.execute(select([PeriodicTaskChanged]).
+        s = connection.execute(select(PeriodicTaskChanged).
                                where(PeriodicTaskChanged.id == 1).limit(1))
         if not s:
             s = connection.execute(insert(PeriodicTaskChanged),
                                    last_update=dt.datetime.now())
         else:
             s = connection.execute(update(PeriodicTaskChanged).
                                    where(PeriodicTaskChanged.id == 1).
@@ -213,15 +251,18 @@
         if periodic_tasks:
             return periodic_tasks.last_update
 
 
 class PeriodicTask(ModelBase, ModelMixin):
 
     __tablename__ = 'celery_periodic_task'
-    __table_args__ = {'sqlite_autoincrement': True}
+    __table_args__ = {
+        'sqlite_autoincrement': True,
+        'schema': 'celery_schema'
+    }
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
     # name
     name = sa.Column(sa.String(255), unique=True)
     # task name
     task = sa.Column(sa.String(255))
 
@@ -243,14 +284,21 @@
     solar_id = sa.Column(sa.Integer)
     solar = relationship(
         SolarSchedule,
         uselist=False,
         primaryjoin=foreign(solar_id) == remote(SolarSchedule.id)
     )
 
+    clocked_id = sa.Column(sa.Integer)
+    clocked = relationship(
+        ClockedSchedule,
+        uselist=False,
+        primaryjoin=foreign(clocked_id) == remote(ClockedSchedule.id)
+    )
+
     args = sa.Column(sa.Text(), default='[]')
     kwargs = sa.Column(sa.Text(), default='{}')
     # queue for celery
     queue = sa.Column(sa.String(255))
     # exchange for celery
     exchange = sa.Column(sa.String(255))
     # routing_key for celery
@@ -267,22 +315,40 @@
     # 修改时间
     date_changed = sa.Column(sa.DateTime(timezone=True),
                              default=func.now(), onupdate=func.now())
     description = sa.Column(sa.Text(), default='')
 
     no_changes = False
 
+    @classmethod
+    def receive_before_insert(cls, mapper, connection, target):
+        schedule_types = ['interval_id', 'crontab_id', 'solar_id', 'clocked_id']
+        selected_schedule_types = [s for s in schedule_types
+                                   if getattr(target, s)]
+        if len(selected_schedule_types) == 0:
+            raise ValueError(
+                'One of clocked, interval, crontab, or solar '
+                'must be set.'
+            )
+        elif len(selected_schedule_types) > 1:
+            raise ValueError('Only one of clocked, interval, crontab, '
+                             'or solar must be set')
+        if target.clocked_id and not target.one_off:
+            raise ValueError("one_off must be True for clocked schedule")
+
     def __repr__(self):
         fmt = '{0.name}: {{no schedule}}'
         if self.interval:
             fmt = '{0.name}: {0.interval}'
         elif self.crontab:
             fmt = '{0.name}: {0.crontab}'
         elif self.solar:
             fmt = '{0.name}: {0.solar}'
+        elif self.clocked:
+            fmt = '{0.name}: {0.clocked}'
         return fmt.format(self)
 
     @property
     def task_name(self):
         return self.task
 
     @task_name.setter
@@ -293,22 +359,28 @@
     def schedule(self):
         if self.interval:
             return self.interval.schedule
         elif self.crontab:
             return self.crontab.schedule
         elif self.solar:
             return self.solar.schedule
+        elif self.clocked:
+            return self.clocked.schedule
         raise ValueError('{} schedule is None!'.format(self.name))
 
 
 listen(PeriodicTask, 'after_insert', PeriodicTaskChanged.update_changed)
 listen(PeriodicTask, 'after_delete', PeriodicTaskChanged.update_changed)
 listen(PeriodicTask, 'after_update', PeriodicTaskChanged.changed)
+listen(PeriodicTask, 'before_insert', PeriodicTask.receive_before_insert)
 listen(IntervalSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
 listen(IntervalSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
 listen(IntervalSchedule, 'after_update', PeriodicTaskChanged.update_changed)
 listen(CrontabSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
 listen(CrontabSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
 listen(CrontabSchedule, 'after_update', PeriodicTaskChanged.update_changed)
 listen(SolarSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
 listen(SolarSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
 listen(SolarSchedule, 'after_update', PeriodicTaskChanged.update_changed)
+listen(ClockedSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
+listen(ClockedSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
+listen(ClockedSchedule, 'after_update', PeriodicTaskChanged.update_changed)
```

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/schedulers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding=utf-8
 
-import logging
 import datetime as dt
+import logging
+import math
 from multiprocessing.util import Finalize
 
 import sqlalchemy
-from celery import current_app
-from celery import schedules
-from celery.beat import Scheduler, ScheduleEntry
+from celery import current_app, schedules
+from celery.beat import ScheduleEntry, Scheduler
 from celery.utils.log import get_logger
 from celery.utils.time import maybe_make_aware
 from kombu.utils.encoding import safe_repr, safe_str
 from kombu.utils.json import dumps, loads
 
-from .session import session_cleanup
-from .session import SessionManager
-from .models import (
-    PeriodicTask, PeriodicTaskChanged,
-    CrontabSchedule, IntervalSchedule,
-    SolarSchedule,
-)
+from .clockedschedule import clocked
+from .models import (ClockedSchedule, CrontabSchedule, IntervalSchedule,
+                     PeriodicTask, PeriodicTaskChanged, SolarSchedule)
+from .session import SessionManager, session_cleanup
 
 # This scheduler must wake up more frequently than the
 # regular of 5 minutes because it needs to take external
 # changes to the schedule into account.
 DEFAULT_MAX_INTERVAL = 5  # seconds
 
 DEFAULT_BEAT_DBURI = 'sqlite:///schedule.db'
 
+DEFAULT_BEAT_SCHEMA = None
+
 ADD_ENTRY_ERROR = """\
 Cannot add entry %r to database schedule: %r. Contents: %r
 """
 
 
 session_manager = SessionManager()
 # session = session_manager()
@@ -44,14 +43,15 @@
     """Scheduler entry taken from database row."""
 
     model_schedules = (
         # (schedule_type, model_type, model_field)
         (schedules.crontab, CrontabSchedule, 'crontab'),
         (schedules.schedule, IntervalSchedule, 'interval'),
         (schedules.solar, SolarSchedule, 'solar'),
+        (clocked, ClockedSchedule, 'clocked'),
     )
     save_fields = ['last_run_at', 'total_run_count', 'no_changes']
 
     def __init__(self, model, Session, app=None, **kw):
         """Initialize the model entry."""
         self.app = app or current_app._get_current_object()
         self.session = kw.get('session')
@@ -91,14 +91,22 @@
             self.options[option] = value
 
         self.total_run_count = model.total_run_count
         self.enabled = model.enabled
 
         if not model.last_run_at:
             model.last_run_at = self._default_now()
+            # if last_run_at is not set and
+            # model.start_time last_run_at should be in way past.
+            # This will trigger the job to run at start_time
+            # and avoid the heap block.
+            if self.model.start_time:
+                model.last_run_at = model.last_run_at \
+                    - dt.timedelta(days=365 * 30)
+
         self.last_run_at = model.last_run_at
 
         # 因为从数据库读取的 last_run_at 可能没有时区信息，所以这里必须加上时区信息
         self.last_run_at = self.last_run_at.replace(tzinfo=self.app.timezone)
 
         # self.options['expires'] 同理
         # if 'expires' in self.options:
@@ -130,16 +138,17 @@
         # START DATE: only run after the `start_time`, if one exists.
         if self.model.start_time is not None:
             now = maybe_make_aware(self._default_now())
             start_time = self.model.start_time.replace(
                 tzinfo=self.app.timezone)
             if now < start_time:
                 # The datetime is before the start date - don't run.
-                _, delay = self.schedule.is_due(self.last_run_at)
-                # use original delay for re-check
+                delay = math.ceil(
+                    (start_time - now).total_seconds()
+                )
                 return schedules.schedstate(False, delay)
 
         # ONE OFF TASK: Disable one off tasks after they've ran once
         if self.model.one_off and self.model.enabled \
                 and self.model.total_run_count > 0:
             self.model.enabled = False  # disable
             self.model.total_run_count = 0  # Reset
@@ -290,16 +299,18 @@
     _heap_invalidated = False
 
     def __init__(self, *args, **kwargs):
         """Initialize the database scheduler."""
         self.app = kwargs['app']
         self.dburi = kwargs.get('dburi') or self.app.conf.get(
             'beat_dburi') or DEFAULT_BEAT_DBURI
-        self.engine, self.Session = session_manager.create_session(self.dburi)
-        session_manager.prepare_models(self.engine)
+        self.schema = kwargs.get('schema') or self.app.conf.get(
+            'beat_schema') or DEFAULT_BEAT_SCHEMA
+        self.engine, self.Session = session_manager.create_session(self.dburi, schema=self.schema)
+        session_manager.prepare_models(self.engine, schema=self.schema)
 
         self._dirty = set()
         Scheduler.__init__(self, *args, **kwargs)
         self._finalize = Finalize(self, self.sync, exitpriority=5)
         self.max_interval = (kwargs.get('max_interval') or
                              self.app.conf.beat_max_loop_interval or
                              DEFAULT_MAX_INTERVAL)
```

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/session.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from contextlib import contextmanager
 
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import NullPool
+from sqlalchemy.schema import CreateSchema
 
 from kombu.utils.compat import register_after_fork
 
 ModelBase = declarative_base()
 
 
 @contextmanager
@@ -48,25 +49,25 @@
                 return self._engines[dburi]
             except KeyError:
                 engine = self._engines[dburi] = create_engine(dburi, **kwargs)
                 return engine
         else:
             return create_engine(dburi, poolclass=NullPool)
 
-    def create_session(self, dburi, short_lived_sessions=False, **kwargs):
+    def create_session(self, dburi, schema=None, short_lived_sessions=False, **kwargs):
         engine = self.get_engine(dburi, **kwargs)
+        engine = engine.execution_options(schema_translate_map={'celery_schema': schema})
         if self.forked:
             if short_lived_sessions or dburi not in self._sessions:
                 self._sessions[dburi] = sessionmaker(bind=engine)
             return engine, self._sessions[dburi]
         else:
             return engine, sessionmaker(bind=engine)
 
-    def prepare_models(self, engine):
+    def prepare_models(self, engine, schema=None):
         if not self.prepared:
+            if schema:
+                with engine.connect() as connection:
+                    connection.execute(CreateSchema(schema, if_not_exists=True))
+                    connection.commit()
             ModelBase.metadata.create_all(engine)
             self.prepared = True
-
-    def session_factory(self, dburi, **kwargs):
-        engine, session = self.create_session(dburi, **kwargs)
-        self.prepare_models(engine)
-        return session()
```

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/time_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+
+# celery schedstate return None will make it not work
+NEVER_CHECK_TIMEOUT = 100000000
+
+
 # Copied from pytz with some changes
 
 def localize(tzinfo, dt, is_dst=False):
     '''Convert naive time to local time'''
     if dt.tzinfo is not None:
         raise ValueError('Not naive datetime (tzinfo is already set)')
     return dt.replace(tzinfo=tzinfo)
```

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.4.2
+Version: 0.4.4
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -86,15 +86,18 @@
 from celery import Celery
 
 celery = Celery('tasks')
 
 beat_dburi = 'sqlite:///schedule.db'
 
 celery.conf.update(
-    {'beat_dburi': beat_dburi}
+    {
+        'beat_dburi': beat_dburi,
+        'beat_schema': None  # you can make the scheduler tables under different schema (tested for postgresql, not available in sqlite)
+    }
 )
 ```
 
 Also, you can use MySQL or PostgreSQL.
 
 ```Python
 # MySQL: `pip install mysql-connector`
@@ -266,17 +269,18 @@
 2.  As a separate process, start the beat service (specify the
     scheduler):
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## TO BE ADDED LATER
 
-- Add `ClockedSchedule` model
-- Tests
+- ✅ Add `ClockedSchedule` model
+- Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
+- Use Alembic migrations
 
 Any help is appreciated 🙂
 
 ## Acknowledgments
 
 - [django-celery-beat](https://github.com/celery/django-celery-beat)
 - [celerybeatredis](https://github.com/liuliqiang/celerybeatredis)
```

### Comparing `sqlalchemy_celery_beat-0.4.2/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 sqlalchemy_celery_beat/__init__.py
+sqlalchemy_celery_beat/clockedschedule.py
 sqlalchemy_celery_beat/models.py
 sqlalchemy_celery_beat/schedulers.py
 sqlalchemy_celery_beat/session.py
 sqlalchemy_celery_beat/time_utils.py
 sqlalchemy_celery_beat/tzcrontab.py
 sqlalchemy_celery_beat.egg-info/PKG-INFO
 sqlalchemy_celery_beat.egg-info/SOURCES.txt
```

