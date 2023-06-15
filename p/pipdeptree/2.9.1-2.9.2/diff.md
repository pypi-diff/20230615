# Comparing `tmp/pipdeptree-2.9.1.tar.gz` & `tmp/pipdeptree-2.9.2.tar.gz`

## Comparing `pipdeptree-2.9.1.tar` & `pipdeptree-2.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/tox.ini
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/workflows/check.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/workflows/release.yml
--rw-r--r--   0        0        0    38762 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/src/pipdeptree/version.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/LICENSE
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/README.md
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/pyproject.toml
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/CHANGES.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/tox.ini
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.github/workflows/check.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0    38780 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/LICENSE
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/README.md
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pipdeptree-2.9.2/PKG-INFO
```

### Comparing `pipdeptree-2.9.1/.pre-commit-config.yaml` & `pipdeptree-2.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/CHANGES.md` & `pipdeptree-2.9.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/tox.ini` & `pipdeptree-2.9.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/.github/workflows/check.yml` & `pipdeptree-2.9.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/.github/workflows/release.yml` & `pipdeptree-2.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/src/pipdeptree/__init__.py` & `pipdeptree-2.9.2/src/pipdeptree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -991,15 +991,16 @@
 def _get_args():
     parser = get_parser()
     return parser.parse_args()
 
 
 def handle_non_host_target(args):
     # if target is not current python re-invoke it under the actual host
-    if Path(args.python).absolute() != Path(sys.executable).absolute():
+    py_path = Path(args.python).absolute()
+    if py_path != Path(sys.executable).absolute():
         # there's no way to guarantee that graphviz is available, so refuse
         if args.output_format:
             print(  # noqa: T201
                 "graphviz functionality is not supported when querying non-host python",
                 file=sys.stderr,
             )
             raise SystemExit(1)
@@ -1013,15 +1014,15 @@
 
         main_file = inspect.getsourcefile(sys.modules[__name__])
         with tempfile.TemporaryDirectory() as project:
             shutil.copytree(Path(main_file).parent, Path(project) / "pipdeptree")
             # invoke from an empty folder to avoid cwd altering sys.path
             env = os.environ.copy()
             env["PYTHONPATH"] = project
-            cmd = [args.python, "-m", "pipdeptree"]
+            cmd = [py_path, "-m", "pipdeptree"]
             cmd.extend(argv)
             return subprocess.call(cmd, cwd=project, env=env)  # noqa: S603
     return None
 
 
 def get_installed_distributions(local_only=False, user_only=False):  # noqa: FBT002
     try:
```

### Comparing `pipdeptree-2.9.1/tests/test_pipdeptree.py` & `pipdeptree-2.9.2/tests/test_pipdeptree.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,35 @@
 import random
 import subprocess
 import sys
 from itertools import chain
 from pathlib import Path
 from textwrap import dedent, indent
 from typing import TYPE_CHECKING, Any
-
-try:
-    from unittest import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 
 import pytest
 import virtualenv
 
-import pipdeptree as p
+from pipdeptree import (
+    DistPackage,
+    PackageDAG,
+    ReqPackage,
+    ReversedPackageDAG,
+    conflicting_deps,
+    cyclic_deps,
+    dump_graphviz,
+    get_parser,
+    main,
+    print_graphviz,
+    render_conflicts_text,
+    render_cycles_text,
+    render_mermaid,
+    render_text,
+)
 
 if TYPE_CHECKING:
     from pytest_mock import MockerFixture
 
 # Tests for DAG classes
 
 
@@ -38,15 +49,15 @@
             reqs.append(r)
         m.requires = mock.Mock(return_value=reqs)
         yield m
 
 
 def mock_package_dag(simple_graph):
     pkgs = list(mock_pkgs(simple_graph))
-    return p.PackageDAG.from_pkgs(pkgs)
+    return PackageDAG.from_pkgs(pkgs)
 
 
 # util for comparing tree contents with a simple graph
 def dag_to_dict(g):
     return {k.key: [v.key for v in vs] for k, vs in g._obj.items()}  # noqa: SLF001
 
 
@@ -133,95 +144,95 @@
     graph = dag_to_dict(t_fnmatch.filter_nodes(None, {"a.*"}))
     assert graph == {"b.a": ["b.b"], "b.b": []}
 
 
 def test_package_dag_reverse():
     t1 = t.reverse()
     expected = {"a": [], "b": ["a", "f"], "c": ["a"], "d": ["b", "c"], "e": ["c", "d", "g"], "f": ["g"], "g": []}
-    assert isinstance(t1, p.ReversedPackageDAG)
+    assert isinstance(t1, ReversedPackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t1))
-    assert all(isinstance(k, p.ReqPackage) for k in t1)
-    assert all(isinstance(v, p.DistPackage) for v in chain.from_iterable(t1.values()))
+    assert all(isinstance(k, ReqPackage) for k in t1)
+    assert all(isinstance(v, DistPackage) for v in chain.from_iterable(t1.values()))
 
     # testing reversal of ReversedPackageDAG instance
     expected = {"a": ["b", "c"], "b": ["d"], "c": ["d", "e"], "d": ["e"], "e": [], "f": ["b"], "g": ["e", "f"]}
     t2 = t1.reverse()
-    assert isinstance(t2, p.PackageDAG)
+    assert isinstance(t2, PackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t2))
-    assert all(isinstance(k, p.DistPackage) for k in t2)
-    assert all(isinstance(v, p.ReqPackage) for v in chain.from_iterable(t2.values()))
+    assert all(isinstance(k, DistPackage) for k in t2)
+    assert all(isinstance(v, ReqPackage) for v in chain.from_iterable(t2.values()))
 
 
 # Tests for Package classes
 #
 # Note: For all render methods, we are only testing for frozen=False
 # as mocks with frozen=True are a lot more complicated
 
 
 def test_dist_package_render_as_root():
     foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
-    dp = p.DistPackage(foo)
+    dp = DistPackage(foo)
     is_frozen = False
     assert dp.render_as_root(is_frozen) == "foo==20.4.1"
 
 
 def test_dist_package_render_as_branch():
     foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
-    rp = p.ReqPackage(bar_req, dist=bar)
-    dp = p.DistPackage(foo).as_parent_of(rp)
+    rp = ReqPackage(bar_req, dist=bar)
+    dp = DistPackage(foo).as_parent_of(rp)
     is_frozen = False
     assert dp.render_as_branch(is_frozen) == "foo==20.4.1 [requires: bar>=4.0]"
 
 
 def test_dist_package_as_parent_of():
     foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
-    dp = p.DistPackage(foo)
+    dp = DistPackage(foo)
     assert dp.req is None
 
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
-    rp = p.ReqPackage(bar_req, dist=bar)
+    rp = ReqPackage(bar_req, dist=bar)
     dp1 = dp.as_parent_of(rp)
     assert dp1._obj == dp._obj  # noqa: SLF001
     assert dp1.req is rp
 
     dp2 = dp.as_parent_of(None)
     assert dp2 is dp
 
 
 def test_dist_package_as_dict():
     foo = mock.Mock(key="foo", project_name="foo", version="1.3.2b1")
-    dp = p.DistPackage(foo)
+    dp = DistPackage(foo)
     result = dp.as_dict()
     expected = {"key": "foo", "package_name": "foo", "installed_version": "1.3.2b1"}
     assert expected == result
 
 
 def test_req_package_render_as_root():
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
-    rp = p.ReqPackage(bar_req, dist=bar)
+    rp = ReqPackage(bar_req, dist=bar)
     is_frozen = False
     assert rp.render_as_root(is_frozen) == "bar==4.1.0"
 
 
 def test_req_package_render_as_branch():
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
-    rp = p.ReqPackage(bar_req, dist=bar)
+    rp = ReqPackage(bar_req, dist=bar)
     is_frozen = False
     assert rp.render_as_branch(is_frozen) == "bar [required: >=4.0, installed: 4.1.0]"
 
 
 def test_req_package_as_dict():
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
-    rp = p.ReqPackage(bar_req, dist=bar)
+    rp = ReqPackage(bar_req, dist=bar)
     result = rp.as_dict()
     expected = {"key": "bar", "package_name": "bar", "installed_version": "4.1.0", "required_version": ">=4.0"}
     assert expected == result
 
 
 # Tests for render_text
 
@@ -466,15 +477,15 @@
         ),
     ],
 )
 def test_render_text(capsys, list_all, reverse, unicode, expected_output):
     tree = t.reverse() if reverse else t
     encoding = "utf-8" if unicode else "ascii"
     with mock.patch("sys.stdout", MockStdout(encoding)):
-        p.render_text(tree, float("inf"), list_all=list_all, frozen=False)
+        render_text(tree, float("inf"), list_all=list_all, frozen=False)
         captured = capsys.readouterr()
         assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 @pytest.mark.parametrize(
     ("unicode", "level", "expected_output"),
     [
@@ -563,15 +574,15 @@
             ],
         ),
     ],
 )
 def test_render_text_given_depth(capsys, unicode, level, expected_output):
     encoding = "utf-8" if unicode else "ascii"
     with mock.patch("sys.stdout", MockStdout(encoding)):
-        p.render_text(t, level)
+        render_text(t, level)
         captured = capsys.readouterr()
         assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 # Tests for graph outputs
 
 
@@ -584,15 +595,15 @@
     for node in randomized_nodes:
         edges = t._obj[node]  # noqa: SLF001
         random.shuffle(edges)
         randomized_graph[node] = edges
     assert set(randomized_graph) == set(t._obj)  # noqa: SLF001
 
     # Create a randomized package tree.
-    randomized_dag = p.PackageDAG(randomized_graph)
+    randomized_dag = PackageDAG(randomized_graph)
     assert len(t) == len(randomized_dag)
     return randomized_dag
 
 
 def test_render_mermaid():
     """Check both the sorted and randomized package tree produces the same sorted Mermaid output.
 
@@ -646,27 +657,27 @@
             f -- ">=3.0.0" --> g
         """,
         ),
         " " * 4,
     ).rstrip()
 
     for package_tree in (t, randomized_dag_copy(t)):
-        output = p.render_mermaid(package_tree)
+        output = render_mermaid(package_tree)
         assert output.rstrip() == nodes + dependency_edges
-        reversed_output = p.render_mermaid(package_tree.reverse())
+        reversed_output = render_mermaid(package_tree.reverse())
         assert reversed_output.rstrip() == nodes + reverse_dependency_edges
 
 
 def test_mermaid_reserved_ids():
     package_tree = mock_package_dag(
         {
             ("click", "3.4.0"): [("click-extra", [(">=", "2.0.0")])],
         },
     )
-    output = p.render_mermaid(package_tree)
+    output = render_mermaid(package_tree)
     assert output == dedent(
         """\
         flowchart TD
             classDef missing stroke-dasharray: 5
             click-extra["click-extra\\n(missing)"]:::missing
             click_0["click\\n3.4.0"]
             click_0 -.-> click-extra
@@ -674,16 +685,16 @@
     )
 
 
 def test_render_dot(capsys):
     # Check both the sorted and randomized package tree produces the same sorted
     # graphviz output.
     for package_tree in (t, randomized_dag_copy(t)):
-        output = p.dump_graphviz(package_tree, output_format="dot")
-        p.print_graphviz(output)
+        output = dump_graphviz(package_tree, output_format="dot")
+        print_graphviz(output)
         out, _ = capsys.readouterr()
         assert out == dedent(
             """\
             digraph {
             \ta -> b [label=">=2.0.0"]
             \ta -> c [label=">=5.7.1"]
             \ta [label="a\\n3.4.0"]
@@ -703,26 +714,26 @@
             }
 
             """,
         )
 
 
 def test_render_pdf(tmp_path: Path, mocker: MockerFixture) -> None:
-    output = p.dump_graphviz(t, output_format="pdf")
+    output = dump_graphviz(t, output_format="pdf")
     res = tmp_path / "file"
-    with pytest.raises(OSError, match="Bad file descriptor"):  # noqa: PT012, SIM117 # because we reopen the file
+    with pytest.raises(OSError, match="Bad file"):  # noqa: PT012, SIM117 # because we reopen the file
         with res.open("wb") as buf:
             mocker.patch.object(sys, "stdout", buf)
-            p.print_graphviz(output)
+            print_graphviz(output)
     assert res.read_bytes()[:4] == b"%PDF"
 
 
 def test_render_svg(capsys):
-    output = p.dump_graphviz(t, output_format="svg")
-    p.print_graphviz(output)
+    output = dump_graphviz(t, output_format="svg")
+    print_graphviz(output)
     out, _ = capsys.readouterr()
     assert out.startswith("<?xml")
     assert "<svg" in out
     assert out.strip().endswith("</svg>")
 
 
 # Test for conflicting deps
@@ -765,18 +776,18 @@
             {},
             [],
         ),
     ],
 )
 def test_conflicting_deps(capsys, mpkgs, expected_keys, expected_output):
     tree = mock_package_dag(mpkgs)
-    result = p.conflicting_deps(tree)
+    result = conflicting_deps(tree)
     result_keys = {k.key: [v.key for v in vs] for k, vs in result.items()}
     assert expected_keys == result_keys
-    p.render_conflicts_text(result)
+    render_conflicts_text(result)
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.err.strip()
 
 
 # Tests for cyclic deps
 
 
@@ -800,71 +811,71 @@
             [],
             [],  # no output expected
         ),
     ],
 )
 def test_cyclic_deps(capsys, mpkgs, expected_keys, expected_output):
     tree = mock_package_dag(mpkgs)
-    result = p.cyclic_deps(tree)
+    result = cyclic_deps(tree)
     result_keys = [(a.key, b.key, c.key) for (a, b, c) in result]
     assert sorted(expected_keys) == sorted(result_keys)
-    p.render_cycles_text(result)
+    render_cycles_text(result)
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.err.strip()
 
 
 # Tests for the argparse parser
 
 
 def test_parser_default():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args([])
     assert not args.json
     assert args.output_format is None
 
 
 def test_parser_j():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args(["-j"])
     assert args.json
     assert args.output_format is None
 
 
 def test_parser_json():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args(["--json"])
     assert args.json
     assert args.output_format is None
 
 
 def test_parser_json_tree():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args(["--json-tree"])
     assert args.json_tree
     assert not args.json
     assert args.output_format is None
 
 
 def test_parser_mermaid():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args(["--mermaid"])
     assert args.mermaid
     assert not args.json
     assert args.output_format is None
 
 
 def test_parser_pdf():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args(["--graph-output", "pdf"])
     assert args.output_format == "pdf"
     assert not args.json
 
 
 def test_parser_svg():
-    parser = p.get_parser()
+    parser = get_parser()
     args = parser.parse_args(["--graph-output", "svg"])
     assert args.output_format == "svg"
     assert not args.json
 
 
 @pytest.mark.parametrize(
     ("should_be_error", "depth_arg", "expected_value"),
@@ -873,31 +884,33 @@
         (True, ["--depth", "string"], None),
         (False, ["-d", "0"], 0),
         (False, ["--depth", "8"], 8),
         (False, [], float("inf")),
     ],
 )
 def test_parser_depth(should_be_error, depth_arg, expected_value):
-    parser = p.get_parser()
+    parser = get_parser()
 
     if should_be_error:
         with pytest.raises(SystemExit):
             parser.parse_args(depth_arg)
     else:
         args = parser.parse_args(depth_arg)
         assert args.depth == expected_value
 
 
 @pytest.mark.parametrize("args_joined", [True, False])
 def test_custom_interpreter(tmp_path, monkeypatch, capfd, args_joined):
-    result = virtualenv.cli_run([str(tmp_path), "--activators", ""])
+    result = virtualenv.cli_run([str(tmp_path / "venv"), "--activators", ""])
     cmd = [sys.executable]
-    cmd += [f"--python={result.creator.exe}"] if args_joined else ["--python", str(result.creator.exe)]
+    monkeypatch.chdir(tmp_path)
+    py = str(result.creator.exe.relative_to(tmp_path))
+    cmd += [f"--python={result.creator.exe}"] if args_joined else ["--python", py]
     monkeypatch.setattr(sys, "argv", cmd)
-    p.main()
+    main()
     out, _ = capfd.readouterr()
     found = {i.split("==")[0] for i in out.splitlines()}
     implementation = platform.python_implementation()
     if implementation == "CPython":
         expected = {"pip", "setuptools", "wheel"}
     elif implementation == "PyPy":
         expected = {"cffi", "greenlet", "pip", "readline", "setuptools", "wheel"}
@@ -905,15 +918,15 @@
         raise ValueError(implementation)
     if sys.version_info >= (3, 12):
         expected -= {"setuptools", "wheel"}
     assert found == expected, out
 
     monkeypatch.setattr(sys, "argv", [*cmd, "--graph-output", "something"])
     with pytest.raises(SystemExit) as context:
-        p.main()
+        main()
     out, err = capfd.readouterr()
     assert context.value.code == 1
     assert not out
     assert err == "graphviz functionality is not supported when querying non-host python\n"
 
 
 def test_guess_version_setuptools():
```

### Comparing `pipdeptree-2.9.1/LICENSE` & `pipdeptree-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/README.md` & `pipdeptree-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/pyproject.toml` & `pipdeptree-2.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.1/PKG-INFO` & `pipdeptree-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.9.1
+Version: 2.9.2
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
```

