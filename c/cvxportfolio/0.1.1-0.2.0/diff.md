# Comparing `tmp/cvxportfolio-0.1.1.tar.gz` & `tmp/cvxportfolio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.1.1.tar", max compression
+gzip compressed data, was "cvxportfolio-0.2.0.tar", max compression
```

## Comparing `cvxportfolio-0.1.1.tar` & `cvxportfolio-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      599 2023-04-08 05:48:25.320984 cvxportfolio-0.1.1/LICENSE
--rw-r--r--   0        0        0     3681 2023-04-12 17:11:34.075141 cvxportfolio-0.1.1/README.md
--rw-r--r--   0        0        0     1100 2023-04-13 03:24:52.226520 cvxportfolio-0.1.1/cvxportfolio/__init__.py
--rw-r--r--   0        0        0     7115 2023-04-12 17:11:34.082324 cvxportfolio-0.1.1/cvxportfolio/constraints.py
--rw-r--r--   0        0        0     7166 2023-04-12 17:11:34.082677 cvxportfolio-0.1.1/cvxportfolio/costs.py
--rw-r--r--   0        0        0     6403 2023-04-12 17:11:34.082887 cvxportfolio-0.1.1/cvxportfolio/data.py
--rw-r--r--   0        0        0     3809 2023-04-12 20:26:08.261760 cvxportfolio-0.1.1/cvxportfolio/estimator.py
--rw-r--r--   0        0        0     1278 2023-04-12 17:11:34.083203 cvxportfolio-0.1.1/cvxportfolio/expression.py
--rw-r--r--   0        0        0    12440 2023-04-12 17:11:34.083454 cvxportfolio-0.1.1/cvxportfolio/policies.py
--rw-r--r--   0        0        0     7758 2023-04-12 17:11:34.083828 cvxportfolio-0.1.1/cvxportfolio/result.py
--rw-r--r--   0        0        0     4339 2023-04-12 17:11:34.084082 cvxportfolio-0.1.1/cvxportfolio/returns.py
--rw-r--r--   0        0        0     7696 2023-04-12 17:11:34.084963 cvxportfolio-0.1.1/cvxportfolio/risks.py
--rw-r--r--   0        0        0     9561 2023-04-12 17:11:34.085683 cvxportfolio-0.1.1/cvxportfolio/simulator.py
--rw-r--r--   0        0        0     2973 2023-04-12 17:11:34.086422 cvxportfolio-0.1.1/cvxportfolio/utils.py
--rw-r--r--   0        0        0      673 2023-04-13 03:24:24.847017 cvxportfolio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 cvxportfolio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-04-08 05:48:25.320984 cvxportfolio-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4079 2023-04-24 03:28:10.413934 cvxportfolio-0.2.0/README.md
+-rw-r--r--   0        0        0     1015 2023-04-24 03:29:00.463719 cvxportfolio-0.2.0/cvxportfolio/__init__.py
+-rw-r--r--   0        0        0     7051 2023-04-22 22:02:01.434393 cvxportfolio-0.2.0/cvxportfolio/constraints.py
+-rw-r--r--   0        0        0    14977 2023-04-22 22:02:01.434783 cvxportfolio-0.2.0/cvxportfolio/costs.py
+-rw-r--r--   0        0        0    16552 2023-04-24 03:15:29.788318 cvxportfolio-0.2.0/cvxportfolio/data.py
+-rw-r--r--   0        0        0      893 2023-04-18 17:41:30.519984 cvxportfolio-0.2.0/cvxportfolio/errors.py
+-rw-r--r--   0        0        0    12075 2023-04-19 19:02:58.141925 cvxportfolio-0.2.0/cvxportfolio/estimator.py
+-rw-r--r--   0        0        0     6018 2023-04-22 05:27:54.567565 cvxportfolio-0.2.0/cvxportfolio/legacy.py
+-rw-r--r--   0        0        0    27168 2023-04-24 03:03:00.921115 cvxportfolio-0.2.0/cvxportfolio/policies.py
+-rw-r--r--   0        0        0    10377 2023-04-24 02:57:04.982404 cvxportfolio-0.2.0/cvxportfolio/result.py
+-rw-r--r--   0        0        0     8679 2023-04-23 12:41:41.143567 cvxportfolio-0.2.0/cvxportfolio/returns.py
+-rw-r--r--   0        0        0    22577 2023-04-23 12:25:43.855388 cvxportfolio-0.2.0/cvxportfolio/risks.py
+-rw-r--r--   0        0        0    27831 2023-04-23 10:56:36.475351 cvxportfolio-0.2.0/cvxportfolio/simulator.py
+-rw-r--r--   0        0        0      675 2023-04-24 03:28:51.326012 cvxportfolio-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 cvxportfolio-0.2.0/PKG-INFO
```

### Comparing `cvxportfolio-0.1.1/LICENSE` & `cvxportfolio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.1.1/cvxportfolio/result.py` & `cvxportfolio-0.2.0/cvxportfolio/result.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,25 +13,153 @@
 # limitations under the License.
 
 from __future__ import print_function
 import collections
 import numpy as np
 import pandas as pd
 import copy
-from .policies import MultiPeriodOpt
+from .legacy import *
+from .policies import SinglePeriodOpt, MultiPeriodOpt
+from .estimator import Estimator
+
+__all__ = ['BackTest', 'SimulationResult']
+
+class BacktestResult(Estimator):
+    """This will be the class returned by the simulator.
+
+    It defines a bunch of metrics (Sharpe, ...) that are properties
+    computed from its attribytes. It uses the Estimator logic to update
+    its values by running its registered Simulator class.
+
+    Attributes:
+        w (pd.DataFrame): pre-trade weights
+        z (pd.DataFrame): trade weights
+        v (pd.Series): value of the portfolio
+
+    """
+
+    pass
 
 
 def getFiscalQuarter(dt):
     """Convert a time to a fiscal quarter."""
     year = dt.year
     quarter = (dt.month - 1) // 3 + 1
     return "Q%i %s" % (quarter, year)
+    
+    
+class CommonComputations(BacktestResult):
+    """Temporary while having both old and new interface."""
+
+    @property
+    def v(self):
+        """The value of the portfolio over time."""
+        return self.h.sum(axis=1)
+
+    @property
+    def profit(self):
+        """The profit made, in dollars."""
+        return self.v[-1] - self.v[0]
+
+    @property
+    def w(self):
+        """The weights of the portfolio over time."""
+        return (self.h.T / self.v).T
+
+    @property
+    def leverage(self):
+        """Portfolio leverage"""
+        return np.abs(self.w).sum(1)
+
+    @property
+    def volatility(self):
+        """The annualized, realized portfolio volatility."""
+        return np.sqrt(self.PPY) * np.std(self.returns)
+
+    @property
+    def mean_return(self):
+        """The annualized mean portfolio return."""
+        return self.PPY * np.mean(self.returns)
 
+    @property
+    def returns(self):
+        """The returns R_t = (v_{t+1}-v_t)/v_t"""
+        val = self.v
+        return pd.Series(
+            data=val.values[1:] / val.values[:-1] - 1, index=val.index[:-1]
+        )
+
+    @property
+    def growth_rates(self):
+        """The growth rate log(v_{t+1}/v_t)"""
+        return np.log(self.returns + 1)
+
+    @property
+    def annual_growth_rate(self):
+        """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)"""
+        return self.growth_rates.sum() * self.PPY / self.growth_rates.size
+
+    @property
+    def annual_return(self):
+        """The annualized return in percent."""
+        ret = self.growth_rates
+        return self._growth_to_return(ret.mean())
+
+    def _growth_to_return(self, growth):
+        """Convert growth to annualized percentage return."""
+        return 100 * (np.exp(self.PPY * growth) - 1)
+
+    def get_quarterly_returns(self, benchmark=None):
+        """The annualized returns for each fiscal quarter."""
+        ret = self.growth_rates
+        quarters = ret.groupby(getFiscalQuarter).aggregate(np.mean)
+        return self._growth_to_return(quarters)
+
+    def get_best_quarter(self, benchmark=None):
+        ret = self.get_quarterly_returns(benchmark)
+        return (ret.argmax(), ret.max())
+
+    def get_worst_quarter(self, benchmark=None):
+        ret = self.get_quarterly_returns(benchmark)
+        return (ret.argmin(), ret.min())
+
+    @property
+    def sharpe_ratio(self):
+        return (
+            np.sqrt(self.PPY)
+            * np.mean(self.excess_returns)
+            / np.std(self.excess_returns)
+        )
+
+    @property
+    def turnover(self):
+        """Turnover ||u_t||_1/v_t"""
+        noncash_trades = self.u.drop(self.cash_key, axis=1)
+        return np.abs(noncash_trades).sum(axis=1) / self.v.loc[self.u.index]
+
+    @property
+    def trading_days(self):
+        """The fraction of days with nonzero turnover."""
+        return (self.turnover.values > 0).sum() / self.turnover.size
+
+    @property
+    def max_drawdown(self):
+        """The maximum peak to trough drawdown in percent."""
+        val_arr = self.v.values
+        max_dd_so_far = 0
+        cur_max = val_arr[0]
+        for val in val_arr[1:]:
+            if val >= cur_max:
+                cur_max = val
+            elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
+                max_dd_so_far = 100 * (cur_max - val) / cur_max
+        return max_dd_so_far
 
-class SimulationResult:
+
+class SimulationResult(CommonComputations):
     """A container for the result of a simulation.
 
     Attributes:
         h_next: A dataframe of holdings over time.
         u: A dataframe of trades over time.
         tcosts: A series of transaction costs over time.
         borrow_costs: A series of borrow costs over time.
@@ -101,26 +229,30 @@
 
     def log_policy(self, t, exec_time):
         self.log_data("policy_time", t, exec_time)
         # TODO mpo policy requires changes in the optimization_log methods
         if not isinstance(self.policy, MultiPeriodOpt):
             for cost in self.policy.costs:
                 self.log_data(
-                    "policy_" + cost.__class__.__name__, t, cost.optimization_log(t)
-                )
+                    "policy_" +
+                    cost.__class__.__name__,
+                    t,
+                    cost.optimization_log(t))
 
     def log_simulation(self, t, u, h_next, risk_free_return, exec_time):
         self.log_data("simulation_time", t, exec_time)
         self.log_data("u", t, u)
         self.log_data("h_next", t, h_next)
         self.log_data("risk_free_returns", t, risk_free_return)
         for cost in self.simulator.costs:
             self.log_data(
-                "simulator_" + cost.__class__.__name__, t, cost.simulation_log(t)
-            )
+                "simulator_" +
+                cost.__class__.__name__,
+                t,
+                cost.simulation_log(t))
 
     @property
     def h(self):
         """
         Concatenate initial portfolio and h_next dataframe.
 
         """
@@ -128,114 +260,53 @@
         tmp.loc["last"] = np.nan
         tmp = self.h_next.shift(1)
         tmp.iloc[0] = self.initial_portfolio
         # TODO fix ?
         # tmp.loc[self.h_next.index[-1] + self.timedelta]=self.h_next.iloc[-1]
         return tmp
 
-    @property
-    def v(self):
-        """The value of the portfolio over time."""
-        return self.h.sum(axis=1)
-
-    @property
-    def profit(self):
-        """The profit made, in dollars."""
-        return self.v[-1] - self.v[0]
-
-    @property
-    def w(self):
-        """The weights of the portfolio over time."""
-        return (self.h.T / self.v).T
-
-    @property
-    def leverage(self):
-        """Portfolio leverage"""
-        return np.abs(self.w).sum(1)
-
-    @property
-    def volatility(self):
-        """The annualized, realized portfolio volatility."""
-        return np.sqrt(self.PPY) * np.std(self.returns)
-
-    @property
-    def mean_return(self):
-        """The annualized mean portfolio return."""
-        return self.PPY * np.mean(self.returns)
-
-    @property
-    def returns(self):
-        """The returns R_t = (v_{t+1}-v_t)/v_t"""
-        val = self.v
-        return pd.Series(
-            data=val.values[1:] / val.values[:-1] - 1, index=val.index[:-1]
-        )
-
-    @property
-    def growth_rates(self):
-        """The growth rate log(v_{t+1}/v_t)"""
-        return np.log(self.returns + 1)
-
-    @property
-    def annual_growth_rate(self):
-        """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)"""
-        return self.growth_rates.sum() * self.PPY / self.growth_rates.size
-
-    @property
-    def annual_return(self):
-        """The annualized return in percent."""
-        ret = self.growth_rates
-        return self._growth_to_return(ret.mean())
-
-    def _growth_to_return(self, growth):
-        """Convert growth to annualized percentage return."""
-        return 100 * (np.exp(self.PPY * growth) - 1)
-
-    def get_quarterly_returns(self, benchmark=None):
-        """The annualized returns for each fiscal quarter."""
-        ret = self.growth_rates
-        quarters = ret.groupby(getFiscalQuarter).aggregate(np.mean)
-        return self._growth_to_return(quarters)
-
-    def get_best_quarter(self, benchmark=None):
-        ret = self.get_quarterly_returns(benchmark)
-        return (ret.argmax(), ret.max())
-
-    def get_worst_quarter(self, benchmark=None):
-        ret = self.get_quarterly_returns(benchmark)
-        return (ret.argmin(), ret.min())
-
+    
+        
+        
+class BackTest(CommonComputations):
+    """Perform a backtest and hold the results."""
+    
+    def __init__(self, policy, simulator, start_time, end_time=None, value_init = 1E6, h=None):
+        
+        self.policy = policy
+        self.simulator = simulator
+        self.start_time = pd.Series(simulator.returns.data.index >= start_time, simulator.returns.data.index).idxmax()
+        if end_time is None:
+            self.end_time  = simulator.returns.data.index[-1]
+        else:
+            self.end_time = simulator.returns.data.index[simulator.returns.data.index <= end_time][-1]
+        
+        self.end_time = end_time
+        simulator.initialize_policy(policy, self.start_time , self.end_time)
+        
+        if h is None:
+            h = pd.Series(0., simulator.returns.data.columns)
+            h[-1] = value_init
+        
+        self.h = pd.DataFrame(columns=simulator.returns.data.columns)
+        self.u = pd.DataFrame(columns=simulator.returns.data.columns)
+        self.z = pd.DataFrame(columns=simulator.returns.data.columns)
+        self.tcost = pd.Series(dtype=float)
+        self.hcost_stocks = pd.Series(dtype=float)
+        self.hcost_cash = pd.Series(dtype=float)
+        
+        for t in simulator.returns.data.index[(simulator.returns.data.index >= self.start_time) & (simulator.returns.data.index < self.end_time)]:
+            self.h.loc[t] = h
+            h, self.z.loc[t], self.u.loc[t], self.tcost.loc[t], self.hcost_stocks.loc[t], self.hcost_cash.loc[t] = \
+                simulator.simulate(t=t, h=h, policy=self.policy)
+        
+        self.h.loc[self.end_time] = h    
+        
+        self.PPY = 252
+        self.timedelta = pd.Timedelta('1d')
+        self.cash_key = self.h.columns[-1]
+        
     @property
     def excess_returns(self):
-        return self.returns - self.risk_free_returns
+        return self.returns - self.simulator.returns.data[self.cash_key].loc[self.returns.index]
 
-    @property
-    def sharpe_ratio(self):
-        return (
-            np.sqrt(self.PPY)
-            * np.mean(self.excess_returns)
-            / np.std(self.excess_returns)
-        )
-
-    @property
-    def turnover(self):
-        """Turnover ||u_t||_1/v_t"""
-        noncash_trades = self.u.drop(self.cash_key, axis=1)
-        return np.abs(noncash_trades).sum(axis=1) / self.v
-
-    @property
-    def trading_days(self):
-        """The fraction of days with nonzero turnover."""
-        return (self.turnover.values > 0).sum() / self.turnover.size
-
-    @property
-    def max_drawdown(self):
-        """The maximum peak to trough drawdown in percent."""
-        val_arr = self.v.values
-        max_dd_so_far = 0
-        cur_max = val_arr[0]
-        for val in val_arr[1:]:
-            if val >= cur_max:
-                cur_max = val
-            elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
-                max_dd_so_far = 100 * (cur_max - val) / cur_max
-        return max_dd_so_far
+
```

### Comparing `cvxportfolio-0.1.1/pyproject.toml` & `cvxportfolio-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxportfolio"
-version = "0.1.1"
+version = "0.2.0"
 description = "..."
 authors = ["Cvxportfolio's Contributors"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxportfolio"
 homepage = "https://cvxportfolio.readthedocs.io"
 packages = [{include = "cvxportfolio"}]
 
@@ -19,14 +19,13 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.0"
 pytest-cov = "*"
 matplotlib = "*" 
 sphinx = "*"
 numpydoc = "*" # for sphinx
-myst-parser = "*"
-jupyter = "*"
-black = "*"
+myst-parser = "*" # for sphinx
+autopep8 = "*"
 
 [build-system]
 requires = ["poetry>=1.0.2"]
 build-backend = "poetry.masonry.api"
```

