# Comparing `tmp/gradio_log-0.0.3.tar.gz` & `tmp/gradio_log-0.0.4.tar.gz`

## Comparing `gradio_log-0.0.3.tar` & `gradio_log-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0  2126108 2020-02-02 00:00:00.000000 gradio_log-0.0.3/assets/dynamic.gif
--rw-r--r--   0        0        0   143801 2020-02-02 00:00:00.000000 gradio_log-0.0.3/assets/static.png
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_log-0.0.3/backend/gradio_log/__init__.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 gradio_log-0.0.3/backend/gradio_log/log.py
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 gradio_log-0.0.3/backend/gradio_log/log.pyi
--rw-r--r--   0        0        0   454722 2020-02-02 00:00:00.000000 gradio_log-0.0.3/backend/gradio_log/templates/component/index.js
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 gradio_log-0.0.3/backend/gradio_log/templates/component/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_log-0.0.3/demo/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 gradio_log-0.0.3/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_log-0.0.3/demo/css.css
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 gradio_log-0.0.3/demo/space.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 gradio_log-0.0.3/frontend/Index.svelte
--rw-r--r--   0        0        0    35719 2020-02-02 00:00:00.000000 gradio_log-0.0.3/frontend/package-lock.json
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gradio_log-0.0.3/frontend/package.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 gradio_log-0.0.3/.gitignore
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 gradio_log-0.0.3/README.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 gradio_log-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 gradio_log-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0  2126108 2020-02-02 00:00:00.000000 gradio_log-0.0.4/assets/dynamic.gif
+-rw-r--r--   0        0        0   143801 2020-02-02 00:00:00.000000 gradio_log-0.0.4/assets/static.png
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_log-0.0.4/backend/gradio_log/__init__.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 gradio_log-0.0.4/backend/gradio_log/log.py
+-rw-r--r--   0        0        0    19916 2020-02-02 00:00:00.000000 gradio_log-0.0.4/backend/gradio_log/log.pyi
+-rw-r--r--   0        0        0   467008 2020-02-02 00:00:00.000000 gradio_log-0.0.4/backend/gradio_log/templates/component/index.js
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 gradio_log-0.0.4/backend/gradio_log/templates/component/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_log-0.0.4/demo/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 gradio_log-0.0.4/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_log-0.0.4/demo/css.css
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 gradio_log-0.0.4/demo/space.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 gradio_log-0.0.4/frontend/Index.svelte
+-rw-r--r--   0        0        0    35719 2020-02-02 00:00:00.000000 gradio_log-0.0.4/frontend/package-lock.json
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gradio_log-0.0.4/frontend/package.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 gradio_log-0.0.4/.gitignore
+-rw-r--r--   0        0        0    15049 2020-02-02 00:00:00.000000 gradio_log-0.0.4/README.md
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 gradio_log-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 gradio_log-0.0.4/PKG-INFO
```

### Comparing `gradio_log-0.0.3/assets/dynamic.gif` & `gradio_log-0.0.4/assets/dynamic.gif`

 * *Files identical despite different names*

### Comparing `gradio_log-0.0.3/assets/static.png` & `gradio_log-0.0.4/assets/static.png`

 * *Files identical despite different names*

### Comparing `gradio_log-0.0.3/backend/gradio_log/log.pyi` & `gradio_log-0.0.4/backend/gradio_log/log.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Callable
 
 from gradio.components.base import FormComponent
 from gradio.events import Events
 
-
 class log(FormComponent):
 
     def find_start_position(self) -> int:
         self.io.seek(0, 2)
         file_size = self.io.tell()
         lines_found = 0
         block_size = 1024
@@ -165,14 +164,52 @@
         return b
 
     def __init__(
         self,
         log_file: str = None,
         tail: int = 100,
         dark: bool = False,
+        xterm_allow_proposed_api: Optional[bool] = False,
+        xterm_allow_transparency: Optional[bool] = False,
+        xterm_alt_click_moves_cursor: Optional[bool] = True,
+        xterm_convert_eol: Optional[bool] = False,
+        xterm_cursor_blink: Optional[bool] = False,
+        xterm_cursor_inactive_style: Literal[
+            "outline", "block", "bar", "underline", "none"
+        ] = "outline",
+        xterm_cursor_style: Literal["block", "underline", "bar"] = "block",
+        xterm_cursor_width: Optional[int] = 1,
+        xterm_custom_glyphs: Optional[bool] = False,
+        xterm_disable_stdin: Optional[bool] = True,
+        xterm_document_override: Optional[Any] = None,
+        xterm_draw_bold_text_in_bright_colors: Optional[bool] = True,
+        xterm_fast_scroll_modifier: Optional[
+            Literal["none", "alt", "ctrl", "shift"]
+        ] = "alt",
+        xterm_fast_scroll_sensitivity: Optional[int] = 1,
+        xterm_font_family: Optional[str] = "courier-new, courier, monospace",
+        xterm_font_size: Optional[int] = 15,
+        xterm_font_weight: Optional[FontWeight] = "normal",
+        xterm_font_weight_bold: Optional[FontWeight] = "bold",
+        xterm_ignore_bracketed_paste_mode: Optional[bool] = False,
+        xterm_letter_spacing: Optional[float] = 0,
+        xterm_line_height: Optional[float] = 1.0,
+        xterm_log_level: Optional[LogLevel] = "info",
+        xterm_mac_option_click_forces_selection: Optional[bool] = False,
+        xterm_mac_option_is_meta: Optional[bool] = False,
+        xterm_minimum_contrast_ratio: Optional[int] = 1,
+        xterm_overview_ruler_width: Optional[int] = 0,
+        xterm_rescale_overlapping_glyphs: Optional[bool] = False,
+        xterm_screen_reader_mode: Optional[bool] = False,
+        xterm_scroll_on_user_input: Optional[bool] = True,
+        xterm_scroll_sensitivity: Optional[int] = 1,
+        xterm_scrollback: Optional[int] = 1000,
+        xterm_smooth_scroll_duration: Optional[int] = 0,
+        xterm_tab_stop_width: Optional[int] = 8,
+        xterm_windows_mode: Optional[bool] = False,
         *,
         label: str | None = None,
         info: str | None = None,
         every: float = 0.3,
         show_label: bool | None = None,
         container: bool = True,
         scale: int | None = None,
@@ -180,14 +217,17 @@
         interactive: bool | None = None,
         visible: bool = True,
         elem_id: str | None = None,
         elem_classes: list[str] | str | None = None,
         render: bool = True,
     ):
         """
+        For all the xterm options, please refer to the xterm.js documentation:
+        https://xtermjs.org/docs/api/terminal/interfaces/iterminaloptions/
+
         Parameters:
             log_file: the log file path to read from.
             tail: from the end of the file, the number of lines to start read from.
             dark: if True, will render the component in dark mode.
             label: The label for this component. Appears above the component and is also used as the header if there are a table of examples for this component. If None and used in a `gr.Interface`, the label will be the name of the parameter this component is assigned to.
             info: additional component description.
             every: New log pulling interval.
@@ -204,14 +244,53 @@
         self.log_file = log_file
         self.tail = tail
         self.dark = dark
         self.current_pos = None
         self.fd = None
         self.stop_reading = False
 
+        self.xterm_allow_proposed_api = xterm_allow_proposed_api
+        self.xterm_allow_transparency = xterm_allow_transparency
+        self.xterm_alt_click_moves_cursor = xterm_alt_click_moves_cursor
+        self.xterm_convert_eol = xterm_convert_eol
+        self.xterm_cursor_blink = xterm_cursor_blink
+        self.xterm_cursor_inactive_style = xterm_cursor_inactive_style
+        self.xterm_cursor_style = xterm_cursor_style
+        self.xterm_cursor_width = xterm_cursor_width
+        self.xterm_custom_glyphs = xterm_custom_glyphs
+        self.xterm_disable_stdin = xterm_disable_stdin
+        self.xterm_document_override = xterm_document_override
+        self.xterm_draw_bold_text_in_bright_colors = (
+            xterm_draw_bold_text_in_bright_colors
+        )
+        self.xterm_fast_scroll_modifier = xterm_fast_scroll_modifier
+        self.xterm_fast_scroll_sensitivity = xterm_fast_scroll_sensitivity
+        self.xterm_font_family = xterm_font_family
+        self.xterm_font_size = xterm_font_size
+        self.xterm_font_weight = xterm_font_weight
+        self.xterm_font_weight_bold = xterm_font_weight_bold
+        self.xterm_ignore_bracketed_paste_mode = xterm_ignore_bracketed_paste_mode
+        self.xterm_letter_spacing = xterm_letter_spacing
+        self.xterm_line_height = xterm_line_height
+        self.xterm_log_level = xterm_log_level
+        self.xterm_mac_option_click_forces_selection = (
+            xterm_mac_option_click_forces_selection
+        )
+        self.xterm_mac_option_is_meta = xterm_mac_option_is_meta
+        self.xterm_minimum_contrast_ratio = xterm_minimum_contrast_ratio
+        self.xterm_overview_ruler_width = xterm_overview_ruler_width
+        self.xterm_rescale_overlapping_glyphs = xterm_rescale_overlapping_glyphs
+        self.xterm_screen_reader_mode = xterm_screen_reader_mode
+        self.xterm_scroll_on_user_input = xterm_scroll_on_user_input
+        self.xterm_scroll_sensitivity = xterm_scroll_sensitivity
+        self.xterm_scrollback = xterm_scrollback
+        self.xterm_smooth_scroll_duration = xterm_smooth_scroll_duration
+        self.xterm_tab_stop_width = xterm_tab_stop_width
+        self.xterm_windows_mode = xterm_windows_mode
+
         super().__init__(
             label=label,
             info=info,
             every=every,
             show_label=show_label,
             container=container,
             scale=scale,
@@ -234,18 +313,18 @@
         self.current_pos = self.find_start_position()
         self.stop_reading = False
 
     def api_info(self) -> dict[str, Any]:
         return {"type": "string"}
 
     def example_payload(self) -> Any:
-        return "Hello!!"
+        pass
 
     def example_value(self) -> Any:
-        return "Hello!!"
+        pass
 
     
     def load(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
         api_name: str | None | Literal[False] = None,
```

### Comparing `gradio_log-0.0.3/backend/gradio_log/templates/component/index.js` & `gradio_log-0.0.4/backend/gradio_log/templates/component/index.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,35 +1,35 @@
 const {
     SvelteComponent: Kt,
     assign: Vt,
     create_slot: Gt,
     detach: Xt,
     element: Jt,
-    get_all_dirty_from_scope: $t,
-    get_slot_changes: Yt,
-    get_spread_update: Zt,
-    init: Qt,
+    get_all_dirty_from_scope: Yt,
+    get_slot_changes: Zt,
+    get_spread_update: Qt,
+    init: $t,
     insert: ei,
     safe_not_equal: ti,
     set_dynamic_element_data: it,
-    set_style: ne,
-    toggle_class: ue,
+    set_style: ae,
+    toggle_class: fe,
     transition_in: Mt,
-    transition_out: xt,
+    transition_out: Tt,
     update_slot_base: ii
 } = window.__gradio__svelte__internal;
 
 function si(E) {
-    let m, S, y;
-    const R = (
+    let f, p, y;
+    const D = (
             /*#slots*/
             E[18].default
         ),
         M = Gt(
-            R,
+            D,
             E,
             /*$$scope*/
             E[17],
             null
         );
     let k = [{
             "data-testid": (
@@ -38,109 +38,109 @@
             )
         }, {
             id: (
                 /*elem_id*/
                 E[2]
             )
         }, {
-            class: S = "block " + /*elem_classes*/
+            class: p = "block " + /*elem_classes*/
                 E[3].join(" ") + " svelte-nl1om8"
         }],
         i = {};
     for (let n = 0; n < k.length; n += 1)
         i = Vt(i, k[n]);
     return {
         c() {
-            m = Jt(
+            f = Jt(
                 /*tag*/
                 E[14]
             ), M && M.c(), it(
                 /*tag*/
                 E[14]
-            )(m, i), ue(
-                m,
+            )(f, i), fe(
+                f,
                 "hidden",
                 /*visible*/
                 E[10] === !1
-            ), ue(
-                m,
+            ), fe(
+                f,
                 "padded",
                 /*padding*/
                 E[6]
-            ), ue(
-                m,
+            ), fe(
+                f,
                 "border_focus",
                 /*border_mode*/
                 E[5] === "focus"
-            ), ue(
-                m,
+            ), fe(
+                f,
                 "border_contrast",
                 /*border_mode*/
                 E[5] === "contrast"
-            ), ue(m, "hide-container", ! /*explicit_call*/
+            ), fe(f, "hide-container", ! /*explicit_call*/
                 E[8] && ! /*container*/
-                E[9]), ne(
-                m,
+                E[9]), ae(
+                f,
                 "height",
                 /*get_dimension*/
                 E[15](
                     /*height*/
                     E[0]
                 )
-            ), ne(m, "width", typeof /*width*/ E[1] == "number" ? `calc(min(${/*width*/
+            ), ae(f, "width", typeof /*width*/ E[1] == "number" ? `calc(min(${/*width*/
       E[1]}px, 100%))` : (
                 /*get_dimension*/
                 E[15](
                     /*width*/
                     E[1]
                 )
-            )), ne(
-                m,
+            )), ae(
+                f,
                 "border-style",
                 /*variant*/
                 E[4]
-            ), ne(
-                m,
+            ), ae(
+                f,
                 "overflow",
                 /*allow_overflow*/
                 E[11] ? "visible" : "hidden"
-            ), ne(
-                m,
+            ), ae(
+                f,
                 "flex-grow",
                 /*scale*/
                 E[12]
-            ), ne(m, "min-width", `calc(min(${/*min_width*/
-      E[13]}px, 100%))`), ne(m, "border-width", "var(--block-border-width)");
+            ), ae(f, "min-width", `calc(min(${/*min_width*/
+      E[13]}px, 100%))`), ae(f, "border-width", "var(--block-border-width)");
         },
         m(n, o) {
-            ei(n, m, o), M && M.m(m, null), y = !0;
+            ei(n, f, o), M && M.m(f, null), y = !0;
         },
         p(n, o) {
             M && M.p && (!y || o & /*$$scope*/
                     131072) && ii(
                     M,
-                    R,
+                    D,
                     n,
                     /*$$scope*/
                     n[17],
-                    y ? Yt(
-                        R,
+                    y ? Zt(
+                        D,
                         /*$$scope*/
                         n[17],
                         o,
                         null
-                    ) : $t(
+                    ) : Yt(
                         /*$$scope*/
                         n[17]
                     ),
                     null
                 ), it(
                     /*tag*/
                     n[14]
-                )(m, i = Zt(k, [
+                )(f, i = Qt(k, [
                     (!y || o & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
                             n[7]
                         )
                     },
@@ -148,189 +148,189 @@
                         4) && {
                         id: (
                             /*elem_id*/
                             n[2]
                         )
                     },
                     (!y || o & /*elem_classes*/
-                        8 && S !== (S = "block " + /*elem_classes*/
+                        8 && p !== (p = "block " + /*elem_classes*/
                             n[3].join(" ") + " svelte-nl1om8")) && {
-                        class: S
+                        class: p
                     }
-                ])), ue(
-                    m,
+                ])), fe(
+                    f,
                     "hidden",
                     /*visible*/
                     n[10] === !1
-                ), ue(
-                    m,
+                ), fe(
+                    f,
                     "padded",
                     /*padding*/
                     n[6]
-                ), ue(
-                    m,
+                ), fe(
+                    f,
                     "border_focus",
                     /*border_mode*/
                     n[5] === "focus"
-                ), ue(
-                    m,
+                ), fe(
+                    f,
                     "border_contrast",
                     /*border_mode*/
                     n[5] === "contrast"
-                ), ue(m, "hide-container", ! /*explicit_call*/
+                ), fe(f, "hide-container", ! /*explicit_call*/
                     n[8] && ! /*container*/
                     n[9]), o & /*height*/
-                1 && ne(
-                    m,
+                1 && ae(
+                    f,
                     "height",
                     /*get_dimension*/
                     n[15](
                         /*height*/
                         n[0]
                     )
                 ), o & /*width*/
-                2 && ne(m, "width", typeof /*width*/ n[1] == "number" ? `calc(min(${/*width*/
+                2 && ae(f, "width", typeof /*width*/ n[1] == "number" ? `calc(min(${/*width*/
       n[1]}px, 100%))` : (
                     /*get_dimension*/
                     n[15](
                         /*width*/
                         n[1]
                     )
                 )), o & /*variant*/
-                16 && ne(
-                    m,
+                16 && ae(
+                    f,
                     "border-style",
                     /*variant*/
                     n[4]
                 ), o & /*allow_overflow*/
-                2048 && ne(
-                    m,
+                2048 && ae(
+                    f,
                     "overflow",
                     /*allow_overflow*/
                     n[11] ? "visible" : "hidden"
                 ), o & /*scale*/
-                4096 && ne(
-                    m,
+                4096 && ae(
+                    f,
                     "flex-grow",
                     /*scale*/
                     n[12]
                 ), o & /*min_width*/
-                8192 && ne(m, "min-width", `calc(min(${/*min_width*/
+                8192 && ae(f, "min-width", `calc(min(${/*min_width*/
       n[13]}px, 100%))`);
         },
         i(n) {
             y || (Mt(M, n), y = !0);
         },
         o(n) {
-            xt(M, n), y = !1;
+            Tt(M, n), y = !1;
         },
         d(n) {
-            n && Xt(m), M && M.d(n);
+            n && Xt(f), M && M.d(n);
         }
     };
 }
 
 function ri(E) {
-    let m, S = (
+    let f, p = (
         /*tag*/
         E[14] && si(E)
     );
     return {
         c() {
-            S && S.c();
+            p && p.c();
         },
-        m(y, R) {
-            S && S.m(y, R), m = !0;
+        m(y, D) {
+            p && p.m(y, D), f = !0;
         },
-        p(y, [R]) {
+        p(y, [D]) {
             /*tag*/
-            y[14] && S.p(y, R);
+            y[14] && p.p(y, D);
         },
         i(y) {
-            m || (Mt(S, y), m = !0);
+            f || (Mt(p, y), f = !0);
         },
         o(y) {
-            xt(S, y), m = !1;
+            Tt(p, y), f = !1;
         },
         d(y) {
-            S && S.d(y);
+            p && p.d(y);
         }
     };
 }
 
-function ni(E, m, S) {
+function ni(E, f, p) {
     let {
         $$slots: y = {},
-        $$scope: R
-    } = m, {
+        $$scope: D
+    } = f, {
         height: M = void 0
-    } = m, {
+    } = f, {
         width: k = void 0
-    } = m, {
+    } = f, {
         elem_id: i = ""
-    } = m, {
+    } = f, {
         elem_classes: n = []
-    } = m, {
+    } = f, {
         variant: o = "solid"
-    } = m, {
+    } = f, {
         border_mode: c = "base"
-    } = m, {
+    } = f, {
         padding: a = !0
-    } = m, {
+    } = f, {
         type: d = "normal"
-    } = m, {
-        test_id: f = void 0
-    } = m, {
-        explicit_call: g = !1
-    } = m, {
+    } = f, {
+        test_id: v = void 0
+    } = f, {
+        explicit_call: m = !1
+    } = f, {
         container: l = !0
-    } = m, {
+    } = f, {
         visible: s = !0
-    } = m, {
+    } = f, {
         allow_overflow: r = !0
-    } = m, {
-        scale: t = null
-    } = m, {
-        min_width: e = 0
-    } = m, h = d === "fieldset" ? "fieldset" : "div";
-    const v = (u) => {
+    } = f, {
+        scale: e = null
+    } = f, {
+        min_width: t = 0
+    } = f, h = d === "fieldset" ? "fieldset" : "div";
+    const g = (u) => {
         if (u !== void 0) {
             if (typeof u == "number")
                 return u + "px";
             if (typeof u == "string")
                 return u;
         }
     };
     return E.$$set = (u) => {
-        "height" in u && S(0, M = u.height), "width" in u && S(1, k = u.width), "elem_id" in u && S(2, i = u.elem_id), "elem_classes" in u && S(3, n = u.elem_classes), "variant" in u && S(4, o = u.variant), "border_mode" in u && S(5, c = u.border_mode), "padding" in u && S(6, a = u.padding), "type" in u && S(16, d = u.type), "test_id" in u && S(7, f = u.test_id), "explicit_call" in u && S(8, g = u.explicit_call), "container" in u && S(9, l = u.container), "visible" in u && S(10, s = u.visible), "allow_overflow" in u && S(11, r = u.allow_overflow), "scale" in u && S(12, t = u.scale), "min_width" in u && S(13, e = u.min_width), "$$scope" in u && S(17, R = u.$$scope);
+        "height" in u && p(0, M = u.height), "width" in u && p(1, k = u.width), "elem_id" in u && p(2, i = u.elem_id), "elem_classes" in u && p(3, n = u.elem_classes), "variant" in u && p(4, o = u.variant), "border_mode" in u && p(5, c = u.border_mode), "padding" in u && p(6, a = u.padding), "type" in u && p(16, d = u.type), "test_id" in u && p(7, v = u.test_id), "explicit_call" in u && p(8, m = u.explicit_call), "container" in u && p(9, l = u.container), "visible" in u && p(10, s = u.visible), "allow_overflow" in u && p(11, r = u.allow_overflow), "scale" in u && p(12, e = u.scale), "min_width" in u && p(13, t = u.min_width), "$$scope" in u && p(17, D = u.$$scope);
     }, [
         M,
         k,
         i,
         n,
         o,
         c,
         a,
-        f,
-        g,
+        v,
+        m,
         l,
         s,
         r,
-        t,
         e,
+        t,
         h,
-        v,
+        g,
         d,
-        R,
+        D,
         y
     ];
 }
 class oi extends Kt {
-    constructor(m) {
-        super(), Qt(this, m, ni, ri, ti, {
+    constructor(f) {
+        super(), $t(this, f, ni, ri, ti, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -352,178 +352,178 @@
     detach: ci,
     element: _i,
     get_all_dirty_from_scope: di,
     get_slot_changes: ui,
     init: fi,
     insert: vi,
     safe_not_equal: gi,
-    transition_in: pi,
-    transition_out: mi,
+    transition_in: mi,
+    transition_out: pi,
     update_slot_base: Si
 } = window.__gradio__svelte__internal;
 
 function bi(E) {
-    let m, S;
+    let f, p;
     const y = (
             /*#slots*/
             E[1].default
         ),
-        R = li(
+        D = li(
             y,
             E,
             /*$$scope*/
             E[0],
             null
         );
     return {
         c() {
-            m = _i("div"), R && R.c(), hi(m, "class", "svelte-1hnfib2");
+            f = _i("div"), D && D.c(), hi(f, "class", "svelte-1hnfib2");
         },
         m(M, k) {
-            vi(M, m, k), R && R.m(m, null), S = !0;
+            vi(M, f, k), D && D.m(f, null), p = !0;
         },
         p(M, [k]) {
-            R && R.p && (!S || k & /*$$scope*/
+            D && D.p && (!p || k & /*$$scope*/
                 1) && Si(
-                R,
+                D,
                 y,
                 M,
                 /*$$scope*/
                 M[0],
-                S ? ui(
+                p ? ui(
                     y,
                     /*$$scope*/
                     M[0],
                     k,
                     null
                 ) : di(
                     /*$$scope*/
                     M[0]
                 ),
                 null
             );
         },
         i(M) {
-            S || (pi(R, M), S = !0);
+            p || (mi(D, M), p = !0);
         },
         o(M) {
-            mi(R, M), S = !1;
+            pi(D, M), p = !1;
         },
         d(M) {
-            M && ci(m), R && R.d(M);
+            M && ci(f), D && D.d(M);
         }
     };
 }
 
-function Ci(E, m, S) {
+function Ci(E, f, p) {
     let {
         $$slots: y = {},
-        $$scope: R
-    } = m;
+        $$scope: D
+    } = f;
     return E.$$set = (M) => {
-        "$$scope" in M && S(0, R = M.$$scope);
-    }, [R, y];
+        "$$scope" in M && p(0, D = M.$$scope);
+    }, [D, y];
 }
 class wi extends ai {
-    constructor(m) {
-        super(), fi(this, m, Ci, bi, gi, {});
+    constructor(f) {
+        super(), fi(this, f, Ci, bi, gi, {});
     }
 }
 const {
     SvelteComponent: yi,
     attr: st,
     check_outros: Ei,
     create_component: ki,
     create_slot: Li,
-    destroy_component: Di,
-    detach: We,
-    element: Ri,
-    empty: Ai,
-    get_all_dirty_from_scope: Bi,
-    get_slot_changes: Ti,
+    destroy_component: xi,
+    detach: Ne,
+    element: Di,
+    empty: Ri,
+    get_all_dirty_from_scope: Ai,
+    get_slot_changes: Bi,
     group_outros: Mi,
-    init: xi,
-    insert: Ne,
+    init: Ti,
+    insert: Ue,
     mount_component: Oi,
     safe_not_equal: Pi,
     set_data: Ii,
     space: Hi,
     text: Fi,
-    toggle_class: Ce,
-    transition_in: xe,
-    transition_out: Ue,
+    toggle_class: ye,
+    transition_in: Oe,
+    transition_out: je,
     update_slot_base: Wi
 } = window.__gradio__svelte__internal;
 
 function rt(E) {
-    let m, S;
-    return m = new wi({
+    let f, p;
+    return f = new wi({
         props: {
             $$slots: {
                 default: [Ni]
             },
             $$scope: {
                 ctx: E
             }
         }
     }), {
         c() {
-            ki(m.$$.fragment);
+            ki(f.$$.fragment);
         },
-        m(y, R) {
-            Oi(m, y, R), S = !0;
+        m(y, D) {
+            Oi(f, y, D), p = !0;
         },
-        p(y, R) {
+        p(y, D) {
             const M = {};
-            R & /*$$scope, info*/
+            D & /*$$scope, info*/
                 10 && (M.$$scope = {
-                    dirty: R,
+                    dirty: D,
                     ctx: y
-                }), m.$set(M);
+                }), f.$set(M);
         },
         i(y) {
-            S || (xe(m.$$.fragment, y), S = !0);
+            p || (Oe(f.$$.fragment, y), p = !0);
         },
         o(y) {
-            Ue(m.$$.fragment, y), S = !1;
+            je(f.$$.fragment, y), p = !1;
         },
         d(y) {
-            Di(m, y);
+            xi(f, y);
         }
     };
 }
 
 function Ni(E) {
-    let m;
+    let f;
     return {
         c() {
-            m = Fi(
+            f = Fi(
                 /*info*/
                 E[1]
             );
         },
-        m(S, y) {
-            Ne(S, m, y);
+        m(p, y) {
+            Ue(p, f, y);
         },
-        p(S, y) {
+        p(p, y) {
             y & /*info*/
                 2 && Ii(
-                    m,
+                    f,
                     /*info*/
-                    S[1]
+                    p[1]
                 );
         },
-        d(S) {
-            S && We(m);
+        d(p) {
+            p && Ne(f);
         }
     };
 }
 
 function Ui(E) {
-    let m, S, y, R;
+    let f, p, y, D;
     const M = (
             /*#slots*/
             E[2].default
         ),
         k = Li(
             M,
             E,
@@ -533,89 +533,89 @@
         );
     let i = (
         /*info*/
         E[1] && rt(E)
     );
     return {
         c() {
-            m = Ri("span"), k && k.c(), S = Hi(), i && i.c(), y = Ai(), st(m, "data-testid", "block-info"), st(m, "class", "svelte-22c38v"), Ce(m, "sr-only", ! /*show_label*/
-                E[0]), Ce(m, "hide", ! /*show_label*/
-                E[0]), Ce(
-                m,
+            f = Di("span"), k && k.c(), p = Hi(), i && i.c(), y = Ri(), st(f, "data-testid", "block-info"), st(f, "class", "svelte-22c38v"), ye(f, "sr-only", ! /*show_label*/
+                E[0]), ye(f, "hide", ! /*show_label*/
+                E[0]), ye(
+                f,
                 "has-info",
                 /*info*/
                 E[1] != null
             );
         },
         m(n, o) {
-            Ne(n, m, o), k && k.m(m, null), Ne(n, S, o), i && i.m(n, o), Ne(n, y, o), R = !0;
+            Ue(n, f, o), k && k.m(f, null), Ue(n, p, o), i && i.m(n, o), Ue(n, y, o), D = !0;
         },
         p(n, [o]) {
-            k && k.p && (!R || o & /*$$scope*/
+            k && k.p && (!D || o & /*$$scope*/
                     8) && Wi(
                     k,
                     M,
                     n,
                     /*$$scope*/
                     n[3],
-                    R ? Ti(
+                    D ? Bi(
                         M,
                         /*$$scope*/
                         n[3],
                         o,
                         null
-                    ) : Bi(
+                    ) : Ai(
                         /*$$scope*/
                         n[3]
                     ),
                     null
-                ), (!R || o & /*show_label*/
-                    1) && Ce(m, "sr-only", ! /*show_label*/
-                    n[0]), (!R || o & /*show_label*/
-                    1) && Ce(m, "hide", ! /*show_label*/
-                    n[0]), (!R || o & /*info*/
-                    2) && Ce(
-                    m,
+                ), (!D || o & /*show_label*/
+                    1) && ye(f, "sr-only", ! /*show_label*/
+                    n[0]), (!D || o & /*show_label*/
+                    1) && ye(f, "hide", ! /*show_label*/
+                    n[0]), (!D || o & /*info*/
+                    2) && ye(
+                    f,
                     "has-info",
                     /*info*/
                     n[1] != null
                 ), /*info*/
                 n[1] ? i ? (i.p(n, o), o & /*info*/
-                    2 && xe(i, 1)) : (i = rt(n), i.c(), xe(i, 1), i.m(y.parentNode, y)) : i && (Mi(), Ue(i, 1, 1, () => {
+                    2 && Oe(i, 1)) : (i = rt(n), i.c(), Oe(i, 1), i.m(y.parentNode, y)) : i && (Mi(), je(i, 1, 1, () => {
                     i = null;
                 }), Ei());
         },
         i(n) {
-            R || (xe(k, n), xe(i), R = !0);
+            D || (Oe(k, n), Oe(i), D = !0);
         },
         o(n) {
-            Ue(k, n), Ue(i), R = !1;
+            je(k, n), je(i), D = !1;
         },
         d(n) {
-            n && (We(m), We(S), We(y)), k && k.d(n), i && i.d(n);
+            n && (Ne(f), Ne(p), Ne(y)), k && k.d(n), i && i.d(n);
         }
     };
 }
 
-function ji(E, m, S) {
+function ji(E, f, p) {
     let {
         $$slots: y = {},
-        $$scope: R
-    } = m, {
+        $$scope: D
+    } = f, {
         show_label: M = !0
-    } = m, {
+    } = f, {
         info: k = void 0
-    } = m;
+    } = f;
     return E.$$set = (i) => {
-        "show_label" in i && S(0, M = i.show_label), "info" in i && S(1, k = i.info), "$$scope" in i && S(3, R = i.$$scope);
-    }, [M, k, y, R];
+        "show_label" in i && p(0, M = i.show_label), "info" in i && p(1, k = i.info), "$$scope" in i && p(3, D = i.$$scope);
+    }, [M, k, y, D];
 }
 class zi extends yi {
-    constructor(m) {
-        super(), xi(this, m, ji, Ui, Pi, {
+    constructor(f) {
+        super(), Ti(this, f, ji, Ui, Pi, {
             show_label: 0,
             info: 1
         });
     }
 }
 const qi = [{
         color: "red",
@@ -949,335 +949,335 @@
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
 qi.reduce(
     (E, {
-        color: m,
-        primary: S,
+        color: f,
+        primary: p,
         secondary: y
     }) => ({
         ...E,
-        [m]: {
-            primary: nt[m][S],
-            secondary: nt[m][y]
+        [f]: {
+            primary: nt[f][p],
+            secondary: nt[f][y]
         }
     }), {}
 );
 
-function ye(E) {
-    let m = ["", "k", "M", "G", "T", "P", "E", "Z"],
-        S = 0;
-    for (; E > 1e3 && S < m.length - 1;)
-        E /= 1e3, S++;
-    let y = m[S];
+function ke(E) {
+    let f = ["", "k", "M", "G", "T", "P", "E", "Z"],
+        p = 0;
+    for (; E > 1e3 && p < f.length - 1;)
+        E /= 1e3, p++;
+    let y = f[p];
     return (Number.isInteger(E) ? E : E.toFixed(1)) + y;
 }
 
-function je() {}
+function ze() {}
 
-function Ki(E, m) {
-    return E != E ? m == m : E !== m || E && typeof E == "object" || typeof E == "function";
+function Ki(E, f) {
+    return E != E ? f == f : E !== f || E && typeof E == "object" || typeof E == "function";
 }
 const Ot = typeof window < "u";
 let ot = Ot ? () => window.performance.now() : () => Date.now(),
-    Pt = Ot ? (E) => requestAnimationFrame(E) : je;
-const ke = /* @__PURE__ */ new Set();
+    Pt = Ot ? (E) => requestAnimationFrame(E) : ze;
+const xe = /* @__PURE__ */ new Set();
 
 function It(E) {
-    ke.forEach((m) => {
-        m.c(E) || (ke.delete(m), m.f());
-    }), ke.size !== 0 && Pt(It);
+    xe.forEach((f) => {
+        f.c(E) || (xe.delete(f), f.f());
+    }), xe.size !== 0 && Pt(It);
 }
 
 function Vi(E) {
-    let m;
-    return ke.size === 0 && Pt(It), {
-        promise: new Promise((S) => {
-            ke.add(m = {
+    let f;
+    return xe.size === 0 && Pt(It), {
+        promise: new Promise((p) => {
+            xe.add(f = {
                 c: E,
-                f: S
+                f: p
             });
         }),
         abort() {
-            ke.delete(m);
+            xe.delete(f);
         }
     };
 }
-const we = [];
+const Ee = [];
 
-function Gi(E, m = je) {
-    let S;
+function Gi(E, f = ze) {
+    let p;
     const y = /* @__PURE__ */ new Set();
 
-    function R(i) {
-        if (Ki(E, i) && (E = i, S)) {
-            const n = !we.length;
+    function D(i) {
+        if (Ki(E, i) && (E = i, p)) {
+            const n = !Ee.length;
             for (const o of y)
-                o[1](), we.push(o, E);
+                o[1](), Ee.push(o, E);
             if (n) {
-                for (let o = 0; o < we.length; o += 2)
-                    we[o][0](we[o + 1]);
-                we.length = 0;
+                for (let o = 0; o < Ee.length; o += 2)
+                    Ee[o][0](Ee[o + 1]);
+                Ee.length = 0;
             }
         }
     }
 
     function M(i) {
-        R(i(E));
+        D(i(E));
     }
 
-    function k(i, n = je) {
+    function k(i, n = ze) {
         const o = [i, n];
-        return y.add(o), y.size === 1 && (S = m(R, M) || je), i(E), () => {
-            y.delete(o), y.size === 0 && S && (S(), S = null);
+        return y.add(o), y.size === 1 && (p = f(D, M) || ze), i(E), () => {
+            y.delete(o), y.size === 0 && p && (p(), p = null);
         };
     }
     return {
-        set: R,
+        set: D,
         update: M,
         subscribe: k
     };
 }
 
 function at(E) {
     return Object.prototype.toString.call(E) === "[object Date]";
 }
 
-function Je(E, m, S, y) {
-    if (typeof S == "number" || at(S)) {
-        const R = y - S,
-            M = (S - m) / (E.dt || 1 / 60),
-            k = E.opts.stiffness * R,
+function Je(E, f, p, y) {
+    if (typeof p == "number" || at(p)) {
+        const D = y - p,
+            M = (p - f) / (E.dt || 1 / 60),
+            k = E.opts.stiffness * D,
             i = E.opts.damping * M,
             n = (k - i) * E.inv_mass,
             o = (M + n) * E.dt;
-        return Math.abs(o) < E.opts.precision && Math.abs(R) < E.opts.precision ? y : (E.settled = !1, at(S) ? new Date(S.getTime() + o) : S + o);
+        return Math.abs(o) < E.opts.precision && Math.abs(D) < E.opts.precision ? y : (E.settled = !1, at(p) ? new Date(p.getTime() + o) : p + o);
     } else {
-        if (Array.isArray(S))
-            return S.map(
-                (R, M) => Je(E, m[M], S[M], y[M])
+        if (Array.isArray(p))
+            return p.map(
+                (D, M) => Je(E, f[M], p[M], y[M])
             );
-        if (typeof S == "object") {
-            const R = {};
-            for (const M in S)
-                R[M] = Je(E, m[M], S[M], y[M]);
-            return R;
+        if (typeof p == "object") {
+            const D = {};
+            for (const M in p)
+                D[M] = Je(E, f[M], p[M], y[M]);
+            return D;
         } else
-            throw new Error(`Cannot spring ${typeof S} values`);
+            throw new Error(`Cannot spring ${typeof p} values`);
     }
 }
 
-function ht(E, m = {}) {
-    const S = Gi(E),
+function ht(E, f = {}) {
+    const p = Gi(E),
         {
             stiffness: y = 0.15,
-            damping: R = 0.8,
+            damping: D = 0.8,
             precision: M = 0.01
-        } = m;
+        } = f;
     let k, i, n, o = E,
         c = E,
         a = 1,
         d = 0,
-        f = !1;
+        v = !1;
 
-    function g(s, r = {}) {
+    function m(s, r = {}) {
         c = s;
-        const t = n = {};
-        return E == null || r.hard || l.stiffness >= 1 && l.damping >= 1 ? (f = !0, k = ot(), o = s, S.set(E = c), Promise.resolve()) : (r.soft && (d = 1 / ((r.soft === !0 ? 0.5 : +r.soft) * 60), a = 0), i || (k = ot(), f = !1, i = Vi((e) => {
-            if (f)
-                return f = !1, i = null, !1;
+        const e = n = {};
+        return E == null || r.hard || l.stiffness >= 1 && l.damping >= 1 ? (v = !0, k = ot(), o = s, p.set(E = c), Promise.resolve()) : (r.soft && (d = 1 / ((r.soft === !0 ? 0.5 : +r.soft) * 60), a = 0), i || (k = ot(), v = !1, i = Vi((t) => {
+            if (v)
+                return v = !1, i = null, !1;
             a = Math.min(a + d, 1);
             const h = {
                     inv_mass: a,
                     opts: l,
                     settled: !0,
-                    dt: (e - k) * 60 / 1e3
+                    dt: (t - k) * 60 / 1e3
                 },
-                v = Je(h, o, E, c);
-            return k = e, o = E, S.set(E = v), h.settled && (i = null), !h.settled;
-        })), new Promise((e) => {
+                g = Je(h, o, E, c);
+            return k = t, o = E, p.set(E = g), h.settled && (i = null), !h.settled;
+        })), new Promise((t) => {
             i.promise.then(() => {
-                t === n && e();
+                e === n && t();
             });
         }));
     }
     const l = {
-        set: g,
-        update: (s, r) => g(s(c, E), r),
-        subscribe: S.subscribe,
+        set: m,
+        update: (s, r) => m(s(c, E), r),
+        subscribe: p.subscribe,
         stiffness: y,
-        damping: R,
+        damping: D,
         precision: M
     };
     return l;
 }
 const {
     SvelteComponent: Xi,
-    append: ce,
-    attr: Q,
+    append: _e,
+    attr: te,
     component_subscribe: lt,
     detach: Ji,
-    element: $i,
-    init: Yi,
-    insert: Zi,
+    element: Yi,
+    init: Zi,
+    insert: Qi,
     noop: ct,
-    safe_not_equal: Qi,
-    set_style: He,
-    svg_element: _e,
+    safe_not_equal: $i,
+    set_style: Fe,
+    svg_element: de,
     toggle_class: _t
 } = window.__gradio__svelte__internal, {
     onMount: es
 } = window.__gradio__svelte__internal;
 
 function ts(E) {
-    let m, S, y, R, M, k, i, n, o, c, a, d;
+    let f, p, y, D, M, k, i, n, o, c, a, d;
     return {
         c() {
-            m = $i("div"), S = _e("svg"), y = _e("g"), R = _e("path"), M = _e("path"), k = _e("path"), i = _e("path"), n = _e("g"), o = _e("path"), c = _e("path"), a = _e("path"), d = _e("path"), Q(R, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), Q(R, "fill", "#FF7C00"), Q(R, "fill-opacity", "0.4"), Q(R, "class", "svelte-43sxxs"), Q(M, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), Q(M, "fill", "#FF7C00"), Q(M, "class", "svelte-43sxxs"), Q(k, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), Q(k, "fill", "#FF7C00"), Q(k, "fill-opacity", "0.4"), Q(k, "class", "svelte-43sxxs"), Q(i, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), Q(i, "fill", "#FF7C00"), Q(i, "class", "svelte-43sxxs"), He(y, "transform", "translate(" + /*$top*/
+            f = Yi("div"), p = de("svg"), y = de("g"), D = de("path"), M = de("path"), k = de("path"), i = de("path"), n = de("g"), o = de("path"), c = de("path"), a = de("path"), d = de("path"), te(D, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), te(D, "fill", "#FF7C00"), te(D, "fill-opacity", "0.4"), te(D, "class", "svelte-43sxxs"), te(M, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), te(M, "fill", "#FF7C00"), te(M, "class", "svelte-43sxxs"), te(k, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), te(k, "fill", "#FF7C00"), te(k, "fill-opacity", "0.4"), te(k, "class", "svelte-43sxxs"), te(i, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), te(i, "fill", "#FF7C00"), te(i, "class", "svelte-43sxxs"), Fe(y, "transform", "translate(" + /*$top*/
                 E[1][0] + "px, " + /*$top*/
-                E[1][1] + "px)"), Q(o, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), Q(o, "fill", "#FF7C00"), Q(o, "fill-opacity", "0.4"), Q(o, "class", "svelte-43sxxs"), Q(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), Q(c, "fill", "#FF7C00"), Q(c, "class", "svelte-43sxxs"), Q(a, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), Q(a, "fill", "#FF7C00"), Q(a, "fill-opacity", "0.4"), Q(a, "class", "svelte-43sxxs"), Q(d, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), Q(d, "fill", "#FF7C00"), Q(d, "class", "svelte-43sxxs"), He(n, "transform", "translate(" + /*$bottom*/
+                E[1][1] + "px)"), te(o, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), te(o, "fill", "#FF7C00"), te(o, "fill-opacity", "0.4"), te(o, "class", "svelte-43sxxs"), te(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), te(c, "fill", "#FF7C00"), te(c, "class", "svelte-43sxxs"), te(a, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), te(a, "fill", "#FF7C00"), te(a, "fill-opacity", "0.4"), te(a, "class", "svelte-43sxxs"), te(d, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), te(d, "fill", "#FF7C00"), te(d, "class", "svelte-43sxxs"), Fe(n, "transform", "translate(" + /*$bottom*/
                 E[2][0] + "px, " + /*$bottom*/
-                E[2][1] + "px)"), Q(S, "viewBox", "-1200 -1200 3000 3000"), Q(S, "fill", "none"), Q(S, "xmlns", "http://www.w3.org/2000/svg"), Q(S, "class", "svelte-43sxxs"), Q(m, "class", "svelte-43sxxs"), _t(
-                m,
+                E[2][1] + "px)"), te(p, "viewBox", "-1200 -1200 3000 3000"), te(p, "fill", "none"), te(p, "xmlns", "http://www.w3.org/2000/svg"), te(p, "class", "svelte-43sxxs"), te(f, "class", "svelte-43sxxs"), _t(
+                f,
                 "margin",
                 /*margin*/
                 E[0]
             );
         },
-        m(f, g) {
-            Zi(f, m, g), ce(m, S), ce(S, y), ce(y, R), ce(y, M), ce(y, k), ce(y, i), ce(S, n), ce(n, o), ce(n, c), ce(n, a), ce(n, d);
+        m(v, m) {
+            Qi(v, f, m), _e(f, p), _e(p, y), _e(y, D), _e(y, M), _e(y, k), _e(y, i), _e(p, n), _e(n, o), _e(n, c), _e(n, a), _e(n, d);
         },
-        p(f, [g]) {
-            g & /*$top*/
-                2 && He(y, "transform", "translate(" + /*$top*/
-                    f[1][0] + "px, " + /*$top*/
-                    f[1][1] + "px)"), g & /*$bottom*/
-                4 && He(n, "transform", "translate(" + /*$bottom*/
-                    f[2][0] + "px, " + /*$bottom*/
-                    f[2][1] + "px)"), g & /*margin*/
+        p(v, [m]) {
+            m & /*$top*/
+                2 && Fe(y, "transform", "translate(" + /*$top*/
+                    v[1][0] + "px, " + /*$top*/
+                    v[1][1] + "px)"), m & /*$bottom*/
+                4 && Fe(n, "transform", "translate(" + /*$bottom*/
+                    v[2][0] + "px, " + /*$bottom*/
+                    v[2][1] + "px)"), m & /*margin*/
                 1 && _t(
-                    m,
+                    f,
                     "margin",
                     /*margin*/
-                    f[0]
+                    v[0]
                 );
         },
         i: ct,
         o: ct,
-        d(f) {
-            f && Ji(m);
+        d(v) {
+            v && Ji(f);
         }
     };
 }
 
-function is(E, m, S) {
-    let y, R, {
+function is(E, f, p) {
+    let y, D, {
         margin: M = !0
-    } = m;
+    } = f;
     const k = ht([0, 0]);
-    lt(E, k, (d) => S(1, y = d));
+    lt(E, k, (d) => p(1, y = d));
     const i = ht([0, 0]);
-    lt(E, i, (d) => S(2, R = d));
+    lt(E, i, (d) => p(2, D = d));
     let n;
     async function o() {
         await Promise.all([k.set([125, 140]), i.set([-125, -140])]), await Promise.all([k.set([-125, 140]), i.set([125, -140])]), await Promise.all([k.set([-125, 0]), i.set([125, -0])]), await Promise.all([k.set([125, 0]), i.set([-125, 0])]);
     }
     async function c() {
         await o(), n || c();
     }
     async function a() {
         await Promise.all([k.set([125, 0]), i.set([-125, 0])]), c();
     }
     return es(() => (a(), () => n = !0)), E.$$set = (d) => {
-        "margin" in d && S(0, M = d.margin);
-    }, [M, y, R, k, i];
+        "margin" in d && p(0, M = d.margin);
+    }, [M, y, D, k, i];
 }
 class ss extends Xi {
-    constructor(m) {
-        super(), Yi(this, m, is, ts, Qi, {
+    constructor(f) {
+        super(), Zi(this, f, is, ts, $i, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: rs,
-    append: be,
-    attr: fe,
+    append: Ce,
+    attr: ve,
     binding_callbacks: dt,
     check_outros: Ht,
     create_component: ns,
     create_slot: os,
     destroy_component: as,
     destroy_each: Ft,
-    detach: $,
-    element: ge,
-    empty: Re,
-    ensure_array_like: ze,
+    detach: Q,
+    element: me,
+    empty: Ae,
+    ensure_array_like: qe,
     get_all_dirty_from_scope: hs,
     get_slot_changes: ls,
     group_outros: Wt,
     init: cs,
-    insert: Y,
+    insert: $,
     mount_component: _s,
-    noop: $e,
+    noop: Ye,
     safe_not_equal: ds,
-    set_data: le,
-    set_style: Se,
-    space: ve,
-    text: te,
-    toggle_class: he,
-    transition_in: Le,
-    transition_out: De,
+    set_data: ce,
+    set_style: be,
+    space: ge,
+    text: ne,
+    toggle_class: le,
+    transition_in: De,
+    transition_out: Re,
     update_slot_base: us
 } = window.__gradio__svelte__internal, {
     tick: fs
 } = window.__gradio__svelte__internal, {
     onDestroy: vs
 } = window.__gradio__svelte__internal, gs = (E) => ({}), ut = (E) => ({});
 
-function ft(E, m, S) {
+function ft(E, f, p) {
     const y = E.slice();
-    return y[38] = m[S], y[40] = S, y;
+    return y[38] = f[p], y[40] = p, y;
 }
 
-function vt(E, m, S) {
+function vt(E, f, p) {
     const y = E.slice();
-    return y[38] = m[S], y;
+    return y[38] = f[p], y;
 }
 
-function ps(E) {
-    let m, S = (
+function ms(E) {
+    let f, p = (
             /*i18n*/
             E[1]("common.error") + ""
         ),
-        y, R, M;
+        y, D, M;
     const k = (
             /*#slots*/
             E[29].error
         ),
         i = os(
             k,
             E,
             /*$$scope*/
             E[28],
             ut
         );
     return {
         c() {
-            m = ge("span"), y = te(S), R = ve(), i && i.c(), fe(m, "class", "error svelte-1yserjw");
+            f = me("span"), y = ne(p), D = ge(), i && i.c(), ve(f, "class", "error svelte-1yserjw");
         },
         m(n, o) {
-            Y(n, m, o), be(m, y), Y(n, R, o), i && i.m(n, o), M = !0;
+            $(n, f, o), Ce(f, y), $(n, D, o), i && i.m(n, o), M = !0;
         },
         p(n, o) {
             (!M || o[0] & /*i18n*/
-                2) && S !== (S = /*i18n*/
-                n[1]("common.error") + "") && le(y, S), i && i.p && (!M || o[0] & /*$$scope*/
+                2) && p !== (p = /*i18n*/
+                n[1]("common.error") + "") && ce(y, p), i && i.p && (!M || o[0] & /*$$scope*/
                 268435456) && us(
                 i,
                 k,
                 n,
                 /*$$scope*/
                 n[28],
                 M ? ls(
@@ -1290,493 +1290,493 @@
                     /*$$scope*/
                     n[28]
                 ),
                 ut
             );
         },
         i(n) {
-            M || (Le(i, n), M = !0);
+            M || (De(i, n), M = !0);
         },
         o(n) {
-            De(i, n), M = !1;
+            Re(i, n), M = !1;
         },
         d(n) {
-            n && ($(m), $(R)), i && i.d(n);
+            n && (Q(f), Q(D)), i && i.d(n);
         }
     };
 }
 
-function ms(E) {
-    let m, S, y, R, M, k, i, n, o, c = (
+function ps(E) {
+    let f, p, y, D, M, k, i, n, o, c = (
         /*variant*/
         E[8] === "default" && /*show_eta_bar*/
         E[18] && /*show_progress*/
         E[6] === "full" && gt(E)
     );
 
-    function a(e, h) {
+    function a(t, h) {
         if (
             /*progress*/
-            e[7]
+            t[7]
         )
             return Cs;
         if (
             /*queue_position*/
-            e[2] !== null && /*queue_size*/
-            e[3] !== void 0 && /*queue_position*/
-            e[2] >= 0
+            t[2] !== null && /*queue_size*/
+            t[3] !== void 0 && /*queue_position*/
+            t[2] >= 0
         )
             return bs;
         if (
             /*queue_position*/
-            e[2] === 0
+            t[2] === 0
         )
             return Ss;
     }
     let d = a(E),
-        f = d && d(E),
-        g = (
+        v = d && d(E),
+        m = (
             /*timer*/
             E[5] && St(E)
         );
     const l = [ks, Es],
         s = [];
 
-    function r(e, h) {
+    function r(t, h) {
         return (
             /*last_progress_level*/
-            e[15] != null ? 0 : (
+            t[15] != null ? 0 : (
                 /*show_progress*/
-                e[6] === "full" ? 1 : -1
+                t[6] === "full" ? 1 : -1
             )
         );
     }
     ~(M = r(E)) && (k = s[M] = l[M](E));
-    let t = ! /*timer*/
+    let e = ! /*timer*/
         E[5] && Lt(E);
     return {
         c() {
-            c && c.c(), m = ve(), S = ge("div"), f && f.c(), y = ve(), g && g.c(), R = ve(), k && k.c(), i = ve(), t && t.c(), n = Re(), fe(S, "class", "progress-text svelte-1yserjw"), he(
-                S,
+            c && c.c(), f = ge(), p = me("div"), v && v.c(), y = ge(), m && m.c(), D = ge(), k && k.c(), i = ge(), e && e.c(), n = Ae(), ve(p, "class", "progress-text svelte-1yserjw"), le(
+                p,
                 "meta-text-center",
                 /*variant*/
                 E[8] === "center"
-            ), he(
-                S,
+            ), le(
+                p,
                 "meta-text",
                 /*variant*/
                 E[8] === "default"
             );
         },
-        m(e, h) {
-            c && c.m(e, h), Y(e, m, h), Y(e, S, h), f && f.m(S, null), be(S, y), g && g.m(S, null), Y(e, R, h), ~M && s[M].m(e, h), Y(e, i, h), t && t.m(e, h), Y(e, n, h), o = !0;
+        m(t, h) {
+            c && c.m(t, h), $(t, f, h), $(t, p, h), v && v.m(p, null), Ce(p, y), m && m.m(p, null), $(t, D, h), ~M && s[M].m(t, h), $(t, i, h), e && e.m(t, h), $(t, n, h), o = !0;
         },
-        p(e, h) {
+        p(t, h) {
             /*variant*/
-            e[8] === "default" && /*show_eta_bar*/
-                e[18] && /*show_progress*/
-                e[6] === "full" ? c ? c.p(e, h) : (c = gt(e), c.c(), c.m(m.parentNode, m)) : c && (c.d(1), c = null), d === (d = a(e)) && f ? f.p(e, h) : (f && f.d(1), f = d && d(e), f && (f.c(), f.m(S, y))), /*timer*/
-                e[5] ? g ? g.p(e, h) : (g = St(e), g.c(), g.m(S, null)) : g && (g.d(1), g = null), (!o || h[0] & /*variant*/
-                    256) && he(
-                    S,
+            t[8] === "default" && /*show_eta_bar*/
+                t[18] && /*show_progress*/
+                t[6] === "full" ? c ? c.p(t, h) : (c = gt(t), c.c(), c.m(f.parentNode, f)) : c && (c.d(1), c = null), d === (d = a(t)) && v ? v.p(t, h) : (v && v.d(1), v = d && d(t), v && (v.c(), v.m(p, y))), /*timer*/
+                t[5] ? m ? m.p(t, h) : (m = St(t), m.c(), m.m(p, null)) : m && (m.d(1), m = null), (!o || h[0] & /*variant*/
+                    256) && le(
+                    p,
                     "meta-text-center",
                     /*variant*/
-                    e[8] === "center"
+                    t[8] === "center"
                 ), (!o || h[0] & /*variant*/
-                    256) && he(
-                    S,
+                    256) && le(
+                    p,
                     "meta-text",
                     /*variant*/
-                    e[8] === "default"
+                    t[8] === "default"
                 );
-            let v = M;
-            M = r(e), M === v ? ~M && s[M].p(e, h) : (k && (Wt(), De(s[v], 1, 1, () => {
-                    s[v] = null;
-                }), Ht()), ~M ? (k = s[M], k ? k.p(e, h) : (k = s[M] = l[M](e), k.c()), Le(k, 1), k.m(i.parentNode, i)) : k = null), /*timer*/
-                e[5] ? t && (t.d(1), t = null) : t ? t.p(e, h) : (t = Lt(e), t.c(), t.m(n.parentNode, n));
+            let g = M;
+            M = r(t), M === g ? ~M && s[M].p(t, h) : (k && (Wt(), Re(s[g], 1, 1, () => {
+                    s[g] = null;
+                }), Ht()), ~M ? (k = s[M], k ? k.p(t, h) : (k = s[M] = l[M](t), k.c()), De(k, 1), k.m(i.parentNode, i)) : k = null), /*timer*/
+                t[5] ? e && (e.d(1), e = null) : e ? e.p(t, h) : (e = Lt(t), e.c(), e.m(n.parentNode, n));
         },
-        i(e) {
-            o || (Le(k), o = !0);
+        i(t) {
+            o || (De(k), o = !0);
         },
-        o(e) {
-            De(k), o = !1;
+        o(t) {
+            Re(k), o = !1;
         },
-        d(e) {
-            e && ($(m), $(S), $(R), $(i), $(n)), c && c.d(e), f && f.d(), g && g.d(), ~M && s[M].d(e), t && t.d(e);
+        d(t) {
+            t && (Q(f), Q(p), Q(D), Q(i), Q(n)), c && c.d(t), v && v.d(), m && m.d(), ~M && s[M].d(t), e && e.d(t);
         }
     };
 }
 
 function gt(E) {
-    let m, S = `translateX(${/*eta_level*/
+    let f, p = `translateX(${/*eta_level*/
   (E[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            m = ge("div"), fe(m, "class", "eta-bar svelte-1yserjw"), Se(m, "transform", S);
+            f = me("div"), ve(f, "class", "eta-bar svelte-1yserjw"), be(f, "transform", p);
         },
-        m(y, R) {
-            Y(y, m, R);
+        m(y, D) {
+            $(y, f, D);
         },
-        p(y, R) {
-            R[0] & /*eta_level*/
-                131072 && S !== (S = `translateX(${/*eta_level*/
-      (y[17] || 0) * 100 - 100}%)`) && Se(m, "transform", S);
+        p(y, D) {
+            D[0] & /*eta_level*/
+                131072 && p !== (p = `translateX(${/*eta_level*/
+      (y[17] || 0) * 100 - 100}%)`) && be(f, "transform", p);
         },
         d(y) {
-            y && $(m);
+            y && Q(f);
         }
     };
 }
 
 function Ss(E) {
-    let m;
+    let f;
     return {
         c() {
-            m = te("processing |");
+            f = ne("processing |");
         },
-        m(S, y) {
-            Y(S, m, y);
+        m(p, y) {
+            $(p, f, y);
         },
-        p: $e,
-        d(S) {
-            S && $(m);
+        p: Ye,
+        d(p) {
+            p && Q(f);
         }
     };
 }
 
 function bs(E) {
-    let m, S = (
+    let f, p = (
             /*queue_position*/
             E[2] + 1 + ""
         ),
-        y, R, M, k;
+        y, D, M, k;
     return {
         c() {
-            m = te("queue: "), y = te(S), R = te("/"), M = te(
+            f = ne("queue: "), y = ne(p), D = ne("/"), M = ne(
                 /*queue_size*/
                 E[3]
-            ), k = te(" |");
+            ), k = ne(" |");
         },
         m(i, n) {
-            Y(i, m, n), Y(i, y, n), Y(i, R, n), Y(i, M, n), Y(i, k, n);
+            $(i, f, n), $(i, y, n), $(i, D, n), $(i, M, n), $(i, k, n);
         },
         p(i, n) {
             n[0] & /*queue_position*/
-                4 && S !== (S = /*queue_position*/
-                    i[2] + 1 + "") && le(y, S), n[0] & /*queue_size*/
-                8 && le(
+                4 && p !== (p = /*queue_position*/
+                    i[2] + 1 + "") && ce(y, p), n[0] & /*queue_size*/
+                8 && ce(
                     M,
                     /*queue_size*/
                     i[3]
                 );
         },
         d(i) {
-            i && ($(m), $(y), $(R), $(M), $(k));
+            i && (Q(f), Q(y), Q(D), Q(M), Q(k));
         }
     };
 }
 
 function Cs(E) {
-    let m, S = ze(
+    let f, p = qe(
             /*progress*/
             E[7]
         ),
         y = [];
-    for (let R = 0; R < S.length; R += 1)
-        y[R] = mt(vt(E, S, R));
+    for (let D = 0; D < p.length; D += 1)
+        y[D] = pt(vt(E, p, D));
     return {
         c() {
-            for (let R = 0; R < y.length; R += 1)
-                y[R].c();
-            m = Re();
+            for (let D = 0; D < y.length; D += 1)
+                y[D].c();
+            f = Ae();
         },
-        m(R, M) {
+        m(D, M) {
             for (let k = 0; k < y.length; k += 1)
-                y[k] && y[k].m(R, M);
-            Y(R, m, M);
+                y[k] && y[k].m(D, M);
+            $(D, f, M);
         },
-        p(R, M) {
+        p(D, M) {
             if (M[0] & /*progress*/
                 128) {
-                S = ze(
+                p = qe(
                     /*progress*/
-                    R[7]
+                    D[7]
                 );
                 let k;
-                for (k = 0; k < S.length; k += 1) {
-                    const i = vt(R, S, k);
-                    y[k] ? y[k].p(i, M) : (y[k] = mt(i), y[k].c(), y[k].m(m.parentNode, m));
+                for (k = 0; k < p.length; k += 1) {
+                    const i = vt(D, p, k);
+                    y[k] ? y[k].p(i, M) : (y[k] = pt(i), y[k].c(), y[k].m(f.parentNode, f));
                 }
                 for (; k < y.length; k += 1)
                     y[k].d(1);
-                y.length = S.length;
+                y.length = p.length;
             }
         },
-        d(R) {
-            R && $(m), Ft(y, R);
+        d(D) {
+            D && Q(f), Ft(y, D);
         }
     };
 }
 
-function pt(E) {
-    let m, S = (
+function mt(E) {
+    let f, p = (
             /*p*/
             E[38].unit + ""
         ),
-        y, R, M = " ",
+        y, D, M = " ",
         k;
 
     function i(c, a) {
         return (
             /*p*/
             c[38].length != null ? ys : ws
         );
     }
     let n = i(E),
         o = n(E);
     return {
         c() {
-            o.c(), m = ve(), y = te(S), R = te(" | "), k = te(M);
+            o.c(), f = ge(), y = ne(p), D = ne(" | "), k = ne(M);
         },
         m(c, a) {
-            o.m(c, a), Y(c, m, a), Y(c, y, a), Y(c, R, a), Y(c, k, a);
+            o.m(c, a), $(c, f, a), $(c, y, a), $(c, D, a), $(c, k, a);
         },
         p(c, a) {
-            n === (n = i(c)) && o ? o.p(c, a) : (o.d(1), o = n(c), o && (o.c(), o.m(m.parentNode, m))), a[0] & /*progress*/
-                128 && S !== (S = /*p*/
-                    c[38].unit + "") && le(y, S);
+            n === (n = i(c)) && o ? o.p(c, a) : (o.d(1), o = n(c), o && (o.c(), o.m(f.parentNode, f))), a[0] & /*progress*/
+                128 && p !== (p = /*p*/
+                    c[38].unit + "") && ce(y, p);
         },
         d(c) {
-            c && ($(m), $(y), $(R), $(k)), o.d(c);
+            c && (Q(f), Q(y), Q(D), Q(k)), o.d(c);
         }
     };
 }
 
 function ws(E) {
-    let m = ye(
+    let f = ke(
             /*p*/
             E[38].index || 0
         ) + "",
-        S;
+        p;
     return {
         c() {
-            S = te(m);
+            p = ne(f);
         },
-        m(y, R) {
-            Y(y, S, R);
+        m(y, D) {
+            $(y, p, D);
         },
-        p(y, R) {
-            R[0] & /*progress*/
-                128 && m !== (m = ye(
+        p(y, D) {
+            D[0] & /*progress*/
+                128 && f !== (f = ke(
                     /*p*/
                     y[38].index || 0
-                ) + "") && le(S, m);
+                ) + "") && ce(p, f);
         },
         d(y) {
-            y && $(S);
+            y && Q(p);
         }
     };
 }
 
 function ys(E) {
-    let m = ye(
+    let f = ke(
             /*p*/
             E[38].index || 0
         ) + "",
-        S, y, R = ye(
+        p, y, D = ke(
             /*p*/
             E[38].length
         ) + "",
         M;
     return {
         c() {
-            S = te(m), y = te("/"), M = te(R);
+            p = ne(f), y = ne("/"), M = ne(D);
         },
         m(k, i) {
-            Y(k, S, i), Y(k, y, i), Y(k, M, i);
+            $(k, p, i), $(k, y, i), $(k, M, i);
         },
         p(k, i) {
             i[0] & /*progress*/
-                128 && m !== (m = ye(
+                128 && f !== (f = ke(
                     /*p*/
                     k[38].index || 0
-                ) + "") && le(S, m), i[0] & /*progress*/
-                128 && R !== (R = ye(
+                ) + "") && ce(p, f), i[0] & /*progress*/
+                128 && D !== (D = ke(
                     /*p*/
                     k[38].length
-                ) + "") && le(M, R);
+                ) + "") && ce(M, D);
         },
         d(k) {
-            k && ($(S), $(y), $(M));
+            k && (Q(p), Q(y), Q(M));
         }
     };
 }
 
-function mt(E) {
-    let m, S = (
+function pt(E) {
+    let f, p = (
         /*p*/
-        E[38].index != null && pt(E)
+        E[38].index != null && mt(E)
     );
     return {
         c() {
-            S && S.c(), m = Re();
+            p && p.c(), f = Ae();
         },
-        m(y, R) {
-            S && S.m(y, R), Y(y, m, R);
+        m(y, D) {
+            p && p.m(y, D), $(y, f, D);
         },
-        p(y, R) {
+        p(y, D) {
             /*p*/
-            y[38].index != null ? S ? S.p(y, R) : (S = pt(y), S.c(), S.m(m.parentNode, m)) : S && (S.d(1), S = null);
+            y[38].index != null ? p ? p.p(y, D) : (p = mt(y), p.c(), p.m(f.parentNode, f)) : p && (p.d(1), p = null);
         },
         d(y) {
-            y && $(m), S && S.d(y);
+            y && Q(f), p && p.d(y);
         }
     };
 }
 
 function St(E) {
-    let m, S = (
+    let f, p = (
             /*eta*/
             E[0] ? `/${/*formatted_eta*/
     E[19]}` : ""
         ),
-        y, R;
+        y, D;
     return {
         c() {
-            m = te(
+            f = ne(
                 /*formatted_timer*/
                 E[20]
-            ), y = te(S), R = te("s");
+            ), y = ne(p), D = ne("s");
         },
         m(M, k) {
-            Y(M, m, k), Y(M, y, k), Y(M, R, k);
+            $(M, f, k), $(M, y, k), $(M, D, k);
         },
         p(M, k) {
             k[0] & /*formatted_timer*/
-                1048576 && le(
-                    m,
+                1048576 && ce(
+                    f,
                     /*formatted_timer*/
                     M[20]
                 ), k[0] & /*eta, formatted_eta*/
-                524289 && S !== (S = /*eta*/
+                524289 && p !== (p = /*eta*/
                     M[0] ? `/${/*formatted_eta*/
-      M[19]}` : "") && le(y, S);
+      M[19]}` : "") && ce(y, p);
         },
         d(M) {
-            M && ($(m), $(y), $(R));
+            M && (Q(f), Q(y), Q(D));
         }
     };
 }
 
 function Es(E) {
-    let m, S;
-    return m = new ss({
+    let f, p;
+    return f = new ss({
         props: {
             margin: (
                 /*variant*/
                 E[8] === "default"
             )
         }
     }), {
         c() {
-            ns(m.$$.fragment);
+            ns(f.$$.fragment);
         },
-        m(y, R) {
-            _s(m, y, R), S = !0;
+        m(y, D) {
+            _s(f, y, D), p = !0;
         },
-        p(y, R) {
+        p(y, D) {
             const M = {};
-            R[0] & /*variant*/
+            D[0] & /*variant*/
                 256 && (M.margin = /*variant*/
-                    y[8] === "default"), m.$set(M);
+                    y[8] === "default"), f.$set(M);
         },
         i(y) {
-            S || (Le(m.$$.fragment, y), S = !0);
+            p || (De(f.$$.fragment, y), p = !0);
         },
         o(y) {
-            De(m.$$.fragment, y), S = !1;
+            Re(f.$$.fragment, y), p = !1;
         },
         d(y) {
-            as(m, y);
+            as(f, y);
         }
     };
 }
 
 function ks(E) {
-    let m, S, y, R, M, k = `${/*last_progress_level*/
+    let f, p, y, D, M, k = `${/*last_progress_level*/
   E[15] * 100}%`,
         i = (
             /*progress*/
             E[7] != null && bt(E)
         );
     return {
         c() {
-            m = ge("div"), S = ge("div"), i && i.c(), y = ve(), R = ge("div"), M = ge("div"), fe(S, "class", "progress-level-inner svelte-1yserjw"), fe(M, "class", "progress-bar svelte-1yserjw"), Se(M, "width", k), fe(R, "class", "progress-bar-wrap svelte-1yserjw"), fe(m, "class", "progress-level svelte-1yserjw");
+            f = me("div"), p = me("div"), i && i.c(), y = ge(), D = me("div"), M = me("div"), ve(p, "class", "progress-level-inner svelte-1yserjw"), ve(M, "class", "progress-bar svelte-1yserjw"), be(M, "width", k), ve(D, "class", "progress-bar-wrap svelte-1yserjw"), ve(f, "class", "progress-level svelte-1yserjw");
         },
         m(n, o) {
-            Y(n, m, o), be(m, S), i && i.m(S, null), be(m, y), be(m, R), be(R, M), E[30](M);
+            $(n, f, o), Ce(f, p), i && i.m(p, null), Ce(f, y), Ce(f, D), Ce(D, M), E[30](M);
         },
         p(n, o) {
             /*progress*/
-            n[7] != null ? i ? i.p(n, o) : (i = bt(n), i.c(), i.m(S, null)) : i && (i.d(1), i = null), o[0] & /*last_progress_level*/
+            n[7] != null ? i ? i.p(n, o) : (i = bt(n), i.c(), i.m(p, null)) : i && (i.d(1), i = null), o[0] & /*last_progress_level*/
                 32768 && k !== (k = `${/*last_progress_level*/
-      n[15] * 100}%`) && Se(M, "width", k);
+      n[15] * 100}%`) && be(M, "width", k);
         },
-        i: $e,
-        o: $e,
+        i: Ye,
+        o: Ye,
         d(n) {
-            n && $(m), i && i.d(), E[30](null);
+            n && Q(f), i && i.d(), E[30](null);
         }
     };
 }
 
 function bt(E) {
-    let m, S = ze(
+    let f, p = qe(
             /*progress*/
             E[7]
         ),
         y = [];
-    for (let R = 0; R < S.length; R += 1)
-        y[R] = kt(ft(E, S, R));
+    for (let D = 0; D < p.length; D += 1)
+        y[D] = kt(ft(E, p, D));
     return {
         c() {
-            for (let R = 0; R < y.length; R += 1)
-                y[R].c();
-            m = Re();
+            for (let D = 0; D < y.length; D += 1)
+                y[D].c();
+            f = Ae();
         },
-        m(R, M) {
+        m(D, M) {
             for (let k = 0; k < y.length; k += 1)
-                y[k] && y[k].m(R, M);
-            Y(R, m, M);
+                y[k] && y[k].m(D, M);
+            $(D, f, M);
         },
-        p(R, M) {
+        p(D, M) {
             if (M[0] & /*progress_level, progress*/
                 16512) {
-                S = ze(
+                p = qe(
                     /*progress*/
-                    R[7]
+                    D[7]
                 );
                 let k;
-                for (k = 0; k < S.length; k += 1) {
-                    const i = ft(R, S, k);
-                    y[k] ? y[k].p(i, M) : (y[k] = kt(i), y[k].c(), y[k].m(m.parentNode, m));
+                for (k = 0; k < p.length; k += 1) {
+                    const i = ft(D, p, k);
+                    y[k] ? y[k].p(i, M) : (y[k] = kt(i), y[k].c(), y[k].m(f.parentNode, f));
                 }
                 for (; k < y.length; k += 1)
                     y[k].d(1);
-                y.length = S.length;
+                y.length = p.length;
             }
         },
-        d(R) {
-            R && $(m), Ft(y, R);
+        d(D) {
+            D && Q(f), Ft(y, D);
         }
     };
 }
 
 function Ct(E) {
-    let m, S, y, R, M = (
+    let f, p, y, D, M = (
             /*i*/
             E[40] !== 0 && Ls()
         ),
         k = (
             /*p*/
             E[38].desc != null && wt(E)
         ),
@@ -1791,461 +1791,461 @@
         ),
         n = (
             /*progress_level*/
             E[14] != null && Et(E)
         );
     return {
         c() {
-            M && M.c(), m = ve(), k && k.c(), S = ve(), i && i.c(), y = ve(), n && n.c(), R = Re();
+            M && M.c(), f = ge(), k && k.c(), p = ge(), i && i.c(), y = ge(), n && n.c(), D = Ae();
         },
         m(o, c) {
-            M && M.m(o, c), Y(o, m, c), k && k.m(o, c), Y(o, S, c), i && i.m(o, c), Y(o, y, c), n && n.m(o, c), Y(o, R, c);
+            M && M.m(o, c), $(o, f, c), k && k.m(o, c), $(o, p, c), i && i.m(o, c), $(o, y, c), n && n.m(o, c), $(o, D, c);
         },
         p(o, c) {
             /*p*/
-            o[38].desc != null ? k ? k.p(o, c) : (k = wt(o), k.c(), k.m(S.parentNode, S)) : k && (k.d(1), k = null), /*p*/
+            o[38].desc != null ? k ? k.p(o, c) : (k = wt(o), k.c(), k.m(p.parentNode, p)) : k && (k.d(1), k = null), /*p*/
                 o[38].desc != null && /*progress_level*/
                 o[14] && /*progress_level*/
                 o[14][
                     /*i*/
                     o[40]
                 ] != null ? i || (i = yt(), i.c(), i.m(y.parentNode, y)) : i && (i.d(1), i = null), /*progress_level*/
-                o[14] != null ? n ? n.p(o, c) : (n = Et(o), n.c(), n.m(R.parentNode, R)) : n && (n.d(1), n = null);
+                o[14] != null ? n ? n.p(o, c) : (n = Et(o), n.c(), n.m(D.parentNode, D)) : n && (n.d(1), n = null);
         },
         d(o) {
-            o && ($(m), $(S), $(y), $(R)), M && M.d(o), k && k.d(o), i && i.d(o), n && n.d(o);
+            o && (Q(f), Q(p), Q(y), Q(D)), M && M.d(o), k && k.d(o), i && i.d(o), n && n.d(o);
         }
     };
 }
 
 function Ls(E) {
-    let m;
+    let f;
     return {
         c() {
-            m = te(" /");
+            f = ne(" /");
         },
-        m(S, y) {
-            Y(S, m, y);
+        m(p, y) {
+            $(p, f, y);
         },
-        d(S) {
-            S && $(m);
+        d(p) {
+            p && Q(f);
         }
     };
 }
 
 function wt(E) {
-    let m = (
+    let f = (
             /*p*/
             E[38].desc + ""
         ),
-        S;
+        p;
     return {
         c() {
-            S = te(m);
+            p = ne(f);
         },
-        m(y, R) {
-            Y(y, S, R);
+        m(y, D) {
+            $(y, p, D);
         },
-        p(y, R) {
-            R[0] & /*progress*/
-                128 && m !== (m = /*p*/
-                    y[38].desc + "") && le(S, m);
+        p(y, D) {
+            D[0] & /*progress*/
+                128 && f !== (f = /*p*/
+                    y[38].desc + "") && ce(p, f);
         },
         d(y) {
-            y && $(S);
+            y && Q(p);
         }
     };
 }
 
 function yt(E) {
-    let m;
+    let f;
     return {
         c() {
-            m = te("-");
+            f = ne("-");
         },
-        m(S, y) {
-            Y(S, m, y);
+        m(p, y) {
+            $(p, f, y);
         },
-        d(S) {
-            S && $(m);
+        d(p) {
+            p && Q(f);
         }
     };
 }
 
 function Et(E) {
-    let m = (100 * /*progress_level*/
+    let f = (100 * /*progress_level*/
             (E[14][
                 /*i*/
                 E[40]
             ] || 0)).toFixed(1) + "",
-        S, y;
+        p, y;
     return {
         c() {
-            S = te(m), y = te("%");
+            p = ne(f), y = ne("%");
         },
-        m(R, M) {
-            Y(R, S, M), Y(R, y, M);
+        m(D, M) {
+            $(D, p, M), $(D, y, M);
         },
-        p(R, M) {
+        p(D, M) {
             M[0] & /*progress_level*/
-                16384 && m !== (m = (100 * /*progress_level*/
-                    (R[14][
+                16384 && f !== (f = (100 * /*progress_level*/
+                    (D[14][
                         /*i*/
-                        R[40]
-                    ] || 0)).toFixed(1) + "") && le(S, m);
+                        D[40]
+                    ] || 0)).toFixed(1) + "") && ce(p, f);
         },
-        d(R) {
-            R && ($(S), $(y));
+        d(D) {
+            D && (Q(p), Q(y));
         }
     };
 }
 
 function kt(E) {
-    let m, S = (
+    let f, p = (
         /*p*/
         (E[38].desc != null || /*progress_level*/
             E[14] && /*progress_level*/
             E[14][
                 /*i*/
                 E[40]
             ] != null) && Ct(E)
     );
     return {
         c() {
-            S && S.c(), m = Re();
+            p && p.c(), f = Ae();
         },
-        m(y, R) {
-            S && S.m(y, R), Y(y, m, R);
+        m(y, D) {
+            p && p.m(y, D), $(y, f, D);
         },
-        p(y, R) {
+        p(y, D) {
             /*p*/
             y[38].desc != null || /*progress_level*/
                 y[14] && /*progress_level*/
                 y[14][
                     /*i*/
                     y[40]
-                ] != null ? S ? S.p(y, R) : (S = Ct(y), S.c(), S.m(m.parentNode, m)) : S && (S.d(1), S = null);
+                ] != null ? p ? p.p(y, D) : (p = Ct(y), p.c(), p.m(f.parentNode, f)) : p && (p.d(1), p = null);
         },
         d(y) {
-            y && $(m), S && S.d(y);
+            y && Q(f), p && p.d(y);
         }
     };
 }
 
 function Lt(E) {
-    let m, S;
+    let f, p;
     return {
         c() {
-            m = ge("p"), S = te(
+            f = me("p"), p = ne(
                 /*loading_text*/
                 E[9]
-            ), fe(m, "class", "loading svelte-1yserjw");
+            ), ve(f, "class", "loading svelte-1yserjw");
         },
-        m(y, R) {
-            Y(y, m, R), be(m, S);
+        m(y, D) {
+            $(y, f, D), Ce(f, p);
         },
-        p(y, R) {
-            R[0] & /*loading_text*/
-                512 && le(
-                    S,
+        p(y, D) {
+            D[0] & /*loading_text*/
+                512 && ce(
+                    p,
                     /*loading_text*/
                     y[9]
                 );
         },
         d(y) {
-            y && $(m);
+            y && Q(f);
         }
     };
 }
 
-function Ds(E) {
-    let m, S, y, R, M;
-    const k = [ms, ps],
+function xs(E) {
+    let f, p, y, D, M;
+    const k = [ps, ms],
         i = [];
 
     function n(o, c) {
         return (
             /*status*/
             o[4] === "pending" ? 0 : (
                 /*status*/
                 o[4] === "error" ? 1 : -1
             )
         );
     }
-    return ~(S = n(E)) && (y = i[S] = k[S](E)), {
+    return ~(p = n(E)) && (y = i[p] = k[p](E)), {
         c() {
-            m = ge("div"), y && y.c(), fe(m, "class", R = "wrap " + /*variant*/
+            f = me("div"), y && y.c(), ve(f, "class", D = "wrap " + /*variant*/
                 E[8] + " " + /*show_progress*/
-                E[6] + " svelte-1yserjw"), he(m, "hide", ! /*status*/
+                E[6] + " svelte-1yserjw"), le(f, "hide", ! /*status*/
                 E[4] || /*status*/
                 E[4] === "complete" || /*show_progress*/
-                E[6] === "hidden"), he(
-                m,
+                E[6] === "hidden"), le(
+                f,
                 "translucent",
                 /*variant*/
                 E[8] === "center" && /*status*/
                 (E[4] === "pending" || /*status*/
                     E[4] === "error") || /*translucent*/
                 E[11] || /*show_progress*/
                 E[6] === "minimal"
-            ), he(
-                m,
+            ), le(
+                f,
                 "generating",
                 /*status*/
                 E[4] === "generating"
-            ), he(
-                m,
+            ), le(
+                f,
                 "border",
                 /*border*/
                 E[12]
-            ), Se(
-                m,
+            ), be(
+                f,
                 "position",
                 /*absolute*/
                 E[10] ? "absolute" : "static"
-            ), Se(
-                m,
+            ), be(
+                f,
                 "padding",
                 /*absolute*/
                 E[10] ? "0" : "var(--size-8) 0"
             );
         },
         m(o, c) {
-            Y(o, m, c), ~S && i[S].m(m, null), E[31](m), M = !0;
+            $(o, f, c), ~p && i[p].m(f, null), E[31](f), M = !0;
         },
         p(o, c) {
-            let a = S;
-            S = n(o), S === a ? ~S && i[S].p(o, c) : (y && (Wt(), De(i[a], 1, 1, () => {
+            let a = p;
+            p = n(o), p === a ? ~p && i[p].p(o, c) : (y && (Wt(), Re(i[a], 1, 1, () => {
                     i[a] = null;
-                }), Ht()), ~S ? (y = i[S], y ? y.p(o, c) : (y = i[S] = k[S](o), y.c()), Le(y, 1), y.m(m, null)) : y = null), (!M || c[0] & /*variant, show_progress*/
-                    320 && R !== (R = "wrap " + /*variant*/
+                }), Ht()), ~p ? (y = i[p], y ? y.p(o, c) : (y = i[p] = k[p](o), y.c()), De(y, 1), y.m(f, null)) : y = null), (!M || c[0] & /*variant, show_progress*/
+                    320 && D !== (D = "wrap " + /*variant*/
                         o[8] + " " + /*show_progress*/
-                        o[6] + " svelte-1yserjw")) && fe(m, "class", R), (!M || c[0] & /*variant, show_progress, status, show_progress*/
-                    336) && he(m, "hide", ! /*status*/
+                        o[6] + " svelte-1yserjw")) && ve(f, "class", D), (!M || c[0] & /*variant, show_progress, status, show_progress*/
+                    336) && le(f, "hide", ! /*status*/
                     o[4] || /*status*/
                     o[4] === "complete" || /*show_progress*/
                     o[6] === "hidden"), (!M || c[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && he(
-                    m,
+                    2384) && le(
+                    f,
                     "translucent",
                     /*variant*/
                     o[8] === "center" && /*status*/
                     (o[4] === "pending" || /*status*/
                         o[4] === "error") || /*translucent*/
                     o[11] || /*show_progress*/
                     o[6] === "minimal"
                 ), (!M || c[0] & /*variant, show_progress, status*/
-                    336) && he(
-                    m,
+                    336) && le(
+                    f,
                     "generating",
                     /*status*/
                     o[4] === "generating"
                 ), (!M || c[0] & /*variant, show_progress, border*/
-                    4416) && he(
-                    m,
+                    4416) && le(
+                    f,
                     "border",
                     /*border*/
                     o[12]
                 ), c[0] & /*absolute*/
-                1024 && Se(
-                    m,
+                1024 && be(
+                    f,
                     "position",
                     /*absolute*/
                     o[10] ? "absolute" : "static"
                 ), c[0] & /*absolute*/
-                1024 && Se(
-                    m,
+                1024 && be(
+                    f,
                     "padding",
                     /*absolute*/
                     o[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(o) {
-            M || (Le(y), M = !0);
+            M || (De(y), M = !0);
         },
         o(o) {
-            De(y), M = !1;
+            Re(y), M = !1;
         },
         d(o) {
-            o && $(m), ~S && i[S].d(), E[31](null);
+            o && Q(f), ~p && i[p].d(), E[31](null);
         }
     };
 }
-let Fe = [],
+let We = [],
     Xe = !1;
-async function Rs(E, m = !0) {
-    if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && m !== !0)) {
-        if (Fe.push(E), !Xe)
+async function Ds(E, f = !0) {
+    if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && f !== !0)) {
+        if (We.push(E), !Xe)
             Xe = !0;
         else
             return;
         await fs(), requestAnimationFrame(() => {
-            let S = [0, 0];
-            for (let y = 0; y < Fe.length; y++) {
-                const M = Fe[y].getBoundingClientRect();
-                (y === 0 || M.top + window.scrollY <= S[0]) && (S[0] = M.top + window.scrollY, S[1] = y);
+            let p = [0, 0];
+            for (let y = 0; y < We.length; y++) {
+                const M = We[y].getBoundingClientRect();
+                (y === 0 || M.top + window.scrollY <= p[0]) && (p[0] = M.top + window.scrollY, p[1] = y);
             }
             window.scrollTo({
-                top: S[0] - 20,
+                top: p[0] - 20,
                 behavior: "smooth"
-            }), Xe = !1, Fe = [];
+            }), Xe = !1, We = [];
         });
     }
 }
 
-function As(E, m, S) {
+function Rs(E, f, p) {
     let y, {
-            $$slots: R = {},
+            $$slots: D = {},
             $$scope: M
-        } = m,
+        } = f,
         {
             i18n: k
-        } = m,
+        } = f,
         {
             eta: i = null
-        } = m,
+        } = f,
         {
             queue_position: n
-        } = m,
+        } = f,
         {
             queue_size: o
-        } = m,
+        } = f,
         {
             status: c
-        } = m,
+        } = f,
         {
             scroll_to_output: a = !1
-        } = m,
+        } = f,
         {
             timer: d = !0
-        } = m,
+        } = f,
         {
-            show_progress: f = "full"
-        } = m,
+            show_progress: v = "full"
+        } = f,
         {
-            message: g = null
-        } = m,
+            message: m = null
+        } = f,
         {
             progress: l = null
-        } = m,
+        } = f,
         {
             variant: s = "default"
-        } = m,
+        } = f,
         {
             loading_text: r = "Loading..."
-        } = m,
+        } = f,
         {
-            absolute: t = !0
-        } = m,
+            absolute: e = !0
+        } = f,
         {
-            translucent: e = !1
-        } = m,
+            translucent: t = !1
+        } = f,
         {
             border: h = !1
-        } = m,
+        } = f,
         {
-            autoscroll: v
-        } = m,
-        u, p = !1,
+            autoscroll: g
+        } = f,
+        u, S = !1,
         _ = 0,
         b = 0,
-        A = null,
-        T = null,
-        x = 0,
+        R = null,
+        B = null,
+        T = 0,
         L = null,
         H, W = null,
-        U = !0;
-    const K = () => {
-        S(0, i = S(26, A = S(19, D = null))), S(24, _ = performance.now()), S(25, b = 0), p = !0, j();
+        j = !0;
+    const V = () => {
+        p(0, i = p(26, R = p(19, x = null))), p(24, _ = performance.now()), p(25, b = 0), S = !0, z();
     };
 
-    function j() {
+    function z() {
         requestAnimationFrame(() => {
-            S(25, b = (performance.now() - _) / 1e3), p && j();
+            p(25, b = (performance.now() - _) / 1e3), S && z();
         });
     }
 
     function C() {
-        S(25, b = 0), S(0, i = S(26, A = S(19, D = null))), p && (p = !1);
+        p(25, b = 0), p(0, i = p(26, R = p(19, x = null))), S && (S = !1);
     }
     vs(() => {
-        p && C();
+        S && C();
     });
-    let D = null;
+    let x = null;
 
-    function B(I) {
+    function A(I) {
         dt[I ? "unshift" : "push"](() => {
-            W = I, S(16, W), S(7, l), S(14, L), S(15, H);
+            W = I, p(16, W), p(7, l), p(14, L), p(15, H);
         });
     }
 
     function O(I) {
         dt[I ? "unshift" : "push"](() => {
-            u = I, S(13, u);
+            u = I, p(13, u);
         });
     }
     return E.$$set = (I) => {
-        "i18n" in I && S(1, k = I.i18n), "eta" in I && S(0, i = I.eta), "queue_position" in I && S(2, n = I.queue_position), "queue_size" in I && S(3, o = I.queue_size), "status" in I && S(4, c = I.status), "scroll_to_output" in I && S(21, a = I.scroll_to_output), "timer" in I && S(5, d = I.timer), "show_progress" in I && S(6, f = I.show_progress), "message" in I && S(22, g = I.message), "progress" in I && S(7, l = I.progress), "variant" in I && S(8, s = I.variant), "loading_text" in I && S(9, r = I.loading_text), "absolute" in I && S(10, t = I.absolute), "translucent" in I && S(11, e = I.translucent), "border" in I && S(12, h = I.border), "autoscroll" in I && S(23, v = I.autoscroll), "$$scope" in I && S(28, M = I.$$scope);
+        "i18n" in I && p(1, k = I.i18n), "eta" in I && p(0, i = I.eta), "queue_position" in I && p(2, n = I.queue_position), "queue_size" in I && p(3, o = I.queue_size), "status" in I && p(4, c = I.status), "scroll_to_output" in I && p(21, a = I.scroll_to_output), "timer" in I && p(5, d = I.timer), "show_progress" in I && p(6, v = I.show_progress), "message" in I && p(22, m = I.message), "progress" in I && p(7, l = I.progress), "variant" in I && p(8, s = I.variant), "loading_text" in I && p(9, r = I.loading_text), "absolute" in I && p(10, e = I.absolute), "translucent" in I && p(11, t = I.translucent), "border" in I && p(12, h = I.border), "autoscroll" in I && p(23, g = I.autoscroll), "$$scope" in I && p(28, M = I.$$scope);
     }, E.$$.update = () => {
         E.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            218103809 && (i === null && S(0, i = A), i != null && A !== i && (S(27, T = (performance.now() - _) / 1e3 + i), S(19, D = T.toFixed(1)), S(26, A = i))), E.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            167772160 && S(17, x = T === null || T <= 0 || !b ? null : Math.min(b / T, 1)), E.$$.dirty[0] & /*progress*/
-            128 && l != null && S(18, U = !1), E.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (l != null ? S(14, L = l.map((I) => {
+            218103809 && (i === null && p(0, i = R), i != null && R !== i && (p(27, B = (performance.now() - _) / 1e3 + i), p(19, x = B.toFixed(1)), p(26, R = i))), E.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            167772160 && p(17, T = B === null || B <= 0 || !b ? null : Math.min(b / B, 1)), E.$$.dirty[0] & /*progress*/
+            128 && l != null && p(18, j = !1), E.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (l != null ? p(14, L = l.map((I) => {
                 if (I.index != null && I.length != null)
                     return I.index / I.length;
                 if (I.progress != null)
                     return I.progress;
-            })) : S(14, L = null), L ? (S(15, H = L[L.length - 1]), W && (H === 0 ? S(16, W.style.transition = "0", W) : S(16, W.style.transition = "150ms", W))) : S(15, H = void 0)), E.$$.dirty[0] & /*status*/
-            16 && (c === "pending" ? K() : C()), E.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            10493968 && u && a && (c === "pending" || c === "complete") && Rs(u, v), E.$$.dirty[0] & /*status, message*/
+            })) : p(14, L = null), L ? (p(15, H = L[L.length - 1]), W && (H === 0 ? p(16, W.style.transition = "0", W) : p(16, W.style.transition = "150ms", W))) : p(15, H = void 0)), E.$$.dirty[0] & /*status*/
+            16 && (c === "pending" ? V() : C()), E.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            10493968 && u && a && (c === "pending" || c === "complete") && Ds(u, g), E.$$.dirty[0] & /*status, message*/
             4194320, E.$$.dirty[0] & /*timer_diff*/
-            33554432 && S(20, y = b.toFixed(1));
+            33554432 && p(20, y = b.toFixed(1));
     }, [
         i,
         k,
         n,
         o,
         c,
         d,
-        f,
+        v,
         l,
         s,
         r,
-        t,
         e,
+        t,
         h,
         u,
         L,
         H,
         W,
+        T,
+        j,
         x,
-        U,
-        D,
         y,
         a,
+        m,
         g,
-        v,
         _,
         b,
-        A,
-        T,
-        M,
         R,
         B,
+        M,
+        D,
+        A,
         O
     ];
 }
-class Bs extends rs {
-    constructor(m) {
+class As extends rs {
+    constructor(f) {
         super(), cs(
             this,
-            m,
-            As,
-            Ds,
+            f,
+            Rs,
+            xs,
             ds, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 21,
@@ -2268,211 +2268,211 @@
 
 function Nt(E) {
     return E && E.__esModule && Object.prototype.hasOwnProperty.call(E, "default") ? E.default : E;
 }
 var Ut = {
     exports: {}
 };
-(function(E, m) {
-    (function(S, y) {
+(function(E, f) {
+    (function(p, y) {
         E.exports = y();
     })(globalThis, () => (() => {
-        var S = {
+        var p = {
                 4567: function(k, i, n) {
-                    var o = this && this.__decorate || function(t, e, h, v) {
-                            var u, p = arguments.length,
-                                _ = p < 3 ? e : v === null ? v = Object.getOwnPropertyDescriptor(e, h) : v;
+                    var o = this && this.__decorate || function(e, t, h, g) {
+                            var u, S = arguments.length,
+                                _ = S < 3 ? t : g === null ? g = Object.getOwnPropertyDescriptor(t, h) : g;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                _ = Reflect.decorate(t, e, h, v);
+                                _ = Reflect.decorate(e, t, h, g);
                             else
-                                for (var b = t.length - 1; b >= 0; b--)
-                                    (u = t[b]) && (_ = (p < 3 ? u(_) : p > 3 ? u(e, h, _) : u(e, h)) || _);
-                            return p > 3 && _ && Object.defineProperty(e, h, _), _;
+                                for (var b = e.length - 1; b >= 0; b--)
+                                    (u = e[b]) && (_ = (S < 3 ? u(_) : S > 3 ? u(t, h, _) : u(t, h)) || _);
+                            return S > 3 && _ && Object.defineProperty(t, h, _), _;
                         },
-                        c = this && this.__param || function(t, e) {
-                            return function(h, v) {
-                                e(h, v, t);
+                        c = this && this.__param || function(e, t) {
+                            return function(h, g) {
+                                t(h, g, e);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.AccessibilityManager = void 0;
                     const a = n(9042),
                         d = n(9924),
-                        f = n(844),
-                        g = n(4725),
+                        v = n(844),
+                        m = n(4725),
                         l = n(2585),
                         s = n(3656);
-                    let r = i.AccessibilityManager = class extends f.Disposable {
-                        constructor(t, e, h, v) {
-                            super(), this._terminal = t, this._coreBrowserService = h, this._renderService = v, this._rowColumns = /* @__PURE__ */ new WeakMap(), this._liveRegionLineCount = 0, this._charsToConsume = [], this._charsToAnnounce = "", this._accessibilityContainer = this._coreBrowserService.mainDocument.createElement("div"), this._accessibilityContainer.classList.add("xterm-accessibility"), this._rowContainer = this._coreBrowserService.mainDocument.createElement("div"), this._rowContainer.setAttribute("role", "list"), this._rowContainer.classList.add("xterm-accessibility-tree"), this._rowElements = [];
+                    let r = i.AccessibilityManager = class extends v.Disposable {
+                        constructor(e, t, h, g) {
+                            super(), this._terminal = e, this._coreBrowserService = h, this._renderService = g, this._rowColumns = /* @__PURE__ */ new WeakMap(), this._liveRegionLineCount = 0, this._charsToConsume = [], this._charsToAnnounce = "", this._accessibilityContainer = this._coreBrowserService.mainDocument.createElement("div"), this._accessibilityContainer.classList.add("xterm-accessibility"), this._rowContainer = this._coreBrowserService.mainDocument.createElement("div"), this._rowContainer.setAttribute("role", "list"), this._rowContainer.classList.add("xterm-accessibility-tree"), this._rowElements = [];
                             for (let u = 0; u < this._terminal.rows; u++)
                                 this._rowElements[u] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[u]);
                             if (this._topBoundaryFocusListener = (u) => this._handleBoundaryFocus(u, 0), this._bottomBoundaryFocusListener = (u) => this._handleBoundaryFocus(u, 1), this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._refreshRowsDimensions(), this._accessibilityContainer.appendChild(this._rowContainer), this._liveRegion = this._coreBrowserService.mainDocument.createElement("div"), this._liveRegion.classList.add("live-region"), this._liveRegion.setAttribute("aria-live", "assertive"), this._accessibilityContainer.appendChild(this._liveRegion), this._liveRegionDebouncer = this.register(new d.TimeBasedDebouncer(this._renderRows.bind(this))), !this._terminal.element)
                                 throw new Error("Cannot enable accessibility before Terminal.open");
                             this._terminal.element.insertAdjacentElement("afterbegin", this._accessibilityContainer), this.register(this._terminal.onResize((u) => this._handleResize(u.rows))), this.register(this._terminal.onRender((u) => this._refreshRows(u.start, u.end))), this.register(this._terminal.onScroll(() => this._refreshRows())), this.register(this._terminal.onA11yChar((u) => this._handleChar(u))), this.register(this._terminal.onLineFeed(() => this._handleChar(`
-`))), this.register(this._terminal.onA11yTab((u) => this._handleTab(u))), this.register(this._terminal.onKey((u) => this._handleKey(u.key))), this.register(this._terminal.onBlur(() => this._clearLiveRegion())), this.register(this._renderService.onDimensionsChange(() => this._refreshRowsDimensions())), this.register((0, s.addDisposableDomListener)(document, "selectionchange", () => this._handleSelectionChange())), this.register(this._coreBrowserService.onDprChange(() => this._refreshRowsDimensions())), this._refreshRows(), this.register((0, f.toDisposable)(() => {
+`))), this.register(this._terminal.onA11yTab((u) => this._handleTab(u))), this.register(this._terminal.onKey((u) => this._handleKey(u.key))), this.register(this._terminal.onBlur(() => this._clearLiveRegion())), this.register(this._renderService.onDimensionsChange(() => this._refreshRowsDimensions())), this.register((0, s.addDisposableDomListener)(document, "selectionchange", () => this._handleSelectionChange())), this.register(this._coreBrowserService.onDprChange(() => this._refreshRowsDimensions())), this._refreshRows(), this.register((0, v.toDisposable)(() => {
                                 this._accessibilityContainer.remove(), this._rowElements.length = 0;
                             }));
                         }
-                        _handleTab(t) {
-                            for (let e = 0; e < t; e++)
+                        _handleTab(e) {
+                            for (let t = 0; t < e; t++)
                                 this._handleChar(" ");
                         }
-                        _handleChar(t) {
-                            this._liveRegionLineCount < 21 && (this._charsToConsume.length > 0 ? this._charsToConsume.shift() !== t && (this._charsToAnnounce += t) : this._charsToAnnounce += t, t === `
+                        _handleChar(e) {
+                            this._liveRegionLineCount < 21 && (this._charsToConsume.length > 0 ? this._charsToConsume.shift() !== e && (this._charsToAnnounce += e) : this._charsToAnnounce += e, e === `
 ` && (this._liveRegionLineCount++, this._liveRegionLineCount === 21 && (this._liveRegion.textContent += a.tooMuchOutput)));
                         }
                         _clearLiveRegion() {
                             this._liveRegion.textContent = "", this._liveRegionLineCount = 0;
                         }
-                        _handleKey(t) {
-                            this._clearLiveRegion(), new RegExp("\\p{Control}", "u").test(t) || this._charsToConsume.push(t);
+                        _handleKey(e) {
+                            this._clearLiveRegion(), new RegExp("\\p{Control}", "u").test(e) || this._charsToConsume.push(e);
                         }
-                        _refreshRows(t, e) {
-                            this._liveRegionDebouncer.refresh(t, e, this._terminal.rows);
+                        _refreshRows(e, t) {
+                            this._liveRegionDebouncer.refresh(e, t, this._terminal.rows);
                         }
-                        _renderRows(t, e) {
+                        _renderRows(e, t) {
                             const h = this._terminal.buffer,
-                                v = h.lines.length.toString();
-                            for (let u = t; u <= e; u++) {
-                                const p = h.lines.get(h.ydisp + u),
+                                g = h.lines.length.toString();
+                            for (let u = e; u <= t; u++) {
+                                const S = h.lines.get(h.ydisp + u),
                                     _ = [],
-                                    b = (p == null ? void 0 : p.translateToString(!0, void 0, void 0, _)) || "",
-                                    A = (h.ydisp + u + 1).toString(),
-                                    T = this._rowElements[u];
-                                T && (b.length === 0 ? (T.innerText = " ", this._rowColumns.set(T, [0, 1])) : (T.textContent = b, this._rowColumns.set(T, _)), T.setAttribute("aria-posinset", A), T.setAttribute("aria-setsize", v));
+                                    b = (S == null ? void 0 : S.translateToString(!0, void 0, void 0, _)) || "",
+                                    R = (h.ydisp + u + 1).toString(),
+                                    B = this._rowElements[u];
+                                B && (b.length === 0 ? (B.innerText = " ", this._rowColumns.set(B, [0, 1])) : (B.textContent = b, this._rowColumns.set(B, _)), B.setAttribute("aria-posinset", R), B.setAttribute("aria-setsize", g));
                             }
                             this._announceCharacters();
                         }
                         _announceCharacters() {
                             this._charsToAnnounce.length !== 0 && (this._liveRegion.textContent += this._charsToAnnounce, this._charsToAnnounce = "");
                         }
-                        _handleBoundaryFocus(t, e) {
-                            const h = t.target,
-                                v = this._rowElements[e === 0 ? 1 : this._rowElements.length - 2];
-                            if (h.getAttribute("aria-posinset") === (e === 0 ? "1" : `${this._terminal.buffer.lines.length}`) || t.relatedTarget !== v)
+                        _handleBoundaryFocus(e, t) {
+                            const h = e.target,
+                                g = this._rowElements[t === 0 ? 1 : this._rowElements.length - 2];
+                            if (h.getAttribute("aria-posinset") === (t === 0 ? "1" : `${this._terminal.buffer.lines.length}`) || e.relatedTarget !== g)
                                 return;
-                            let u, p;
-                            if (e === 0 ? (u = h, p = this._rowElements.pop(), this._rowContainer.removeChild(p)) : (u = this._rowElements.shift(), p = h, this._rowContainer.removeChild(u)), u.removeEventListener("focus", this._topBoundaryFocusListener), p.removeEventListener("focus", this._bottomBoundaryFocusListener), e === 0) {
+                            let u, S;
+                            if (t === 0 ? (u = h, S = this._rowElements.pop(), this._rowContainer.removeChild(S)) : (u = this._rowElements.shift(), S = h, this._rowContainer.removeChild(u)), u.removeEventListener("focus", this._topBoundaryFocusListener), S.removeEventListener("focus", this._bottomBoundaryFocusListener), t === 0) {
                                 const _ = this._createAccessibilityTreeNode();
                                 this._rowElements.unshift(_), this._rowContainer.insertAdjacentElement("afterbegin", _);
                             } else {
                                 const _ = this._createAccessibilityTreeNode();
                                 this._rowElements.push(_), this._rowContainer.appendChild(_);
                             }
-                            this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._terminal.scrollLines(e === 0 ? -1 : 1), this._rowElements[e === 0 ? 1 : this._rowElements.length - 2].focus(), t.preventDefault(), t.stopImmediatePropagation();
+                            this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._terminal.scrollLines(t === 0 ? -1 : 1), this._rowElements[t === 0 ? 1 : this._rowElements.length - 2].focus(), e.preventDefault(), e.stopImmediatePropagation();
                         }
                         _handleSelectionChange() {
                             var b;
                             if (this._rowElements.length === 0)
                                 return;
-                            const t = document.getSelection();
-                            if (!t)
+                            const e = document.getSelection();
+                            if (!e)
                                 return;
-                            if (t.isCollapsed)
-                                return void(this._rowContainer.contains(t.anchorNode) && this._terminal.clearSelection());
-                            if (!t.anchorNode || !t.focusNode)
+                            if (e.isCollapsed)
+                                return void(this._rowContainer.contains(e.anchorNode) && this._terminal.clearSelection());
+                            if (!e.anchorNode || !e.focusNode)
                                 return void console.error("anchorNode and/or focusNode are null");
-                            let e = {
-                                    node: t.anchorNode,
-                                    offset: t.anchorOffset
+                            let t = {
+                                    node: e.anchorNode,
+                                    offset: e.anchorOffset
                                 },
                                 h = {
-                                    node: t.focusNode,
-                                    offset: t.focusOffset
+                                    node: e.focusNode,
+                                    offset: e.focusOffset
                                 };
-                            if ((e.node.compareDocumentPosition(h.node) & Node.DOCUMENT_POSITION_PRECEDING || e.node === h.node && e.offset > h.offset) && ([e, h] = [h, e]), e.node.compareDocumentPosition(this._rowElements[0]) & (Node.DOCUMENT_POSITION_CONTAINED_BY | Node.DOCUMENT_POSITION_FOLLOWING) && (e = {
+                            if ((t.node.compareDocumentPosition(h.node) & Node.DOCUMENT_POSITION_PRECEDING || t.node === h.node && t.offset > h.offset) && ([t, h] = [h, t]), t.node.compareDocumentPosition(this._rowElements[0]) & (Node.DOCUMENT_POSITION_CONTAINED_BY | Node.DOCUMENT_POSITION_FOLLOWING) && (t = {
                                     node: this._rowElements[0].childNodes[0],
                                     offset: 0
-                                }), !this._rowContainer.contains(e.node))
+                                }), !this._rowContainer.contains(t.node))
                                 return;
-                            const v = this._rowElements.slice(-1)[0];
-                            if (h.node.compareDocumentPosition(v) & (Node.DOCUMENT_POSITION_CONTAINED_BY | Node.DOCUMENT_POSITION_PRECEDING) && (h = {
-                                    node: v,
-                                    offset: ((b = v.textContent) == null ? void 0 : b.length) ?? 0
+                            const g = this._rowElements.slice(-1)[0];
+                            if (h.node.compareDocumentPosition(g) & (Node.DOCUMENT_POSITION_CONTAINED_BY | Node.DOCUMENT_POSITION_PRECEDING) && (h = {
+                                    node: g,
+                                    offset: ((b = g.textContent) == null ? void 0 : b.length) ?? 0
                                 }), !this._rowContainer.contains(h.node))
                                 return;
                             const u = ({
-                                    node: A,
-                                    offset: T
+                                    node: R,
+                                    offset: B
                                 }) => {
-                                    const x = A instanceof Text ? A.parentNode : A;
-                                    let L = parseInt(x == null ? void 0 : x.getAttribute("aria-posinset"), 10) - 1;
+                                    const T = R instanceof Text ? R.parentNode : R;
+                                    let L = parseInt(T == null ? void 0 : T.getAttribute("aria-posinset"), 10) - 1;
                                     if (isNaN(L))
                                         return console.warn("row is invalid. Race condition?"), null;
-                                    const H = this._rowColumns.get(x);
+                                    const H = this._rowColumns.get(T);
                                     if (!H)
                                         return console.warn("columns is null. Race condition?"), null;
-                                    let W = T < H.length ? H[T] : H.slice(-1)[0] + 1;
+                                    let W = B < H.length ? H[B] : H.slice(-1)[0] + 1;
                                     return W >= this._terminal.cols && (++L, W = 0), {
                                         row: L,
                                         column: W
                                     };
                                 },
-                                p = u(e),
+                                S = u(t),
                                 _ = u(h);
-                            if (p && _) {
-                                if (p.row > _.row || p.row === _.row && p.column >= _.column)
+                            if (S && _) {
+                                if (S.row > _.row || S.row === _.row && S.column >= _.column)
                                     throw new Error("invalid range");
-                                this._terminal.select(p.column, p.row, (_.row - p.row) * this._terminal.cols - p.column + _.column);
+                                this._terminal.select(S.column, S.row, (_.row - S.row) * this._terminal.cols - S.column + _.column);
                             }
                         }
-                        _handleResize(t) {
+                        _handleResize(e) {
                             this._rowElements[this._rowElements.length - 1].removeEventListener("focus", this._bottomBoundaryFocusListener);
-                            for (let e = this._rowContainer.children.length; e < this._terminal.rows; e++)
-                                this._rowElements[e] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[e]);
-                            for (; this._rowElements.length > t;)
+                            for (let t = this._rowContainer.children.length; t < this._terminal.rows; t++)
+                                this._rowElements[t] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[t]);
+                            for (; this._rowElements.length > e;)
                                 this._rowContainer.removeChild(this._rowElements.pop());
                             this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._refreshRowsDimensions();
                         }
                         _createAccessibilityTreeNode() {
-                            const t = this._coreBrowserService.mainDocument.createElement("div");
-                            return t.setAttribute("role", "listitem"), t.tabIndex = -1, this._refreshRowDimensions(t), t;
+                            const e = this._coreBrowserService.mainDocument.createElement("div");
+                            return e.setAttribute("role", "listitem"), e.tabIndex = -1, this._refreshRowDimensions(e), e;
                         }
                         _refreshRowsDimensions() {
                             if (this._renderService.dimensions.css.cell.height) {
                                 this._accessibilityContainer.style.width = `${this._renderService.dimensions.css.canvas.width}px`, this._rowElements.length !== this._terminal.rows && this._handleResize(this._terminal.rows);
-                                for (let t = 0; t < this._terminal.rows; t++)
-                                    this._refreshRowDimensions(this._rowElements[t]);
+                                for (let e = 0; e < this._terminal.rows; e++)
+                                    this._refreshRowDimensions(this._rowElements[e]);
                             }
                         }
-                        _refreshRowDimensions(t) {
-                            t.style.height = `${this._renderService.dimensions.css.cell.height}px`;
+                        _refreshRowDimensions(e) {
+                            e.style.height = `${this._renderService.dimensions.css.cell.height}px`;
                         }
                     };
-                    i.AccessibilityManager = r = o([c(1, l.IInstantiationService), c(2, g.ICoreBrowserService), c(3, g.IRenderService)], r);
+                    i.AccessibilityManager = r = o([c(1, l.IInstantiationService), c(2, m.ICoreBrowserService), c(3, m.IRenderService)], r);
                 },
                 3614: (k, i) => {
                     function n(d) {
                         return d.replace(/\r?\n/g, "\r");
                     }
 
-                    function o(d, f) {
-                        return f ? "\x1B[200~" + d + "\x1B[201~" : d;
+                    function o(d, v) {
+                        return v ? "\x1B[200~" + d + "\x1B[201~" : d;
                     }
 
-                    function c(d, f, g, l) {
-                        d = o(d = n(d), g.decPrivateModes.bracketedPasteMode && l.rawOptions.ignoreBracketedPasteMode !== !0), g.triggerDataEvent(d, !0), f.value = "";
+                    function c(d, v, m, l) {
+                        d = o(d = n(d), m.decPrivateModes.bracketedPasteMode && l.rawOptions.ignoreBracketedPasteMode !== !0), m.triggerDataEvent(d, !0), v.value = "";
                     }
 
-                    function a(d, f, g) {
-                        const l = g.getBoundingClientRect(),
+                    function a(d, v, m) {
+                        const l = m.getBoundingClientRect(),
                             s = d.clientX - l.left - 10,
                             r = d.clientY - l.top - 10;
-                        f.style.width = "20px", f.style.height = "20px", f.style.left = `${s}px`, f.style.top = `${r}px`, f.style.zIndex = "1000", f.focus();
+                        v.style.width = "20px", v.style.height = "20px", v.style.left = `${s}px`, v.style.top = `${r}px`, v.style.zIndex = "1000", v.focus();
                     }
                     Object.defineProperty(i, "__esModule", {
                         value: !0
-                    }), i.rightClickHandler = i.moveTextAreaUnderMouseCursor = i.paste = i.handlePasteEvent = i.copyHandler = i.bracketTextForPaste = i.prepareTextForTerminal = void 0, i.prepareTextForTerminal = n, i.bracketTextForPaste = o, i.copyHandler = function(d, f) {
-                        d.clipboardData && d.clipboardData.setData("text/plain", f.selectionText), d.preventDefault();
-                    }, i.handlePasteEvent = function(d, f, g, l) {
-                        d.stopPropagation(), d.clipboardData && c(d.clipboardData.getData("text/plain"), f, g, l);
-                    }, i.paste = c, i.moveTextAreaUnderMouseCursor = a, i.rightClickHandler = function(d, f, g, l, s) {
-                        a(d, f, g), s && l.rightClickSelect(d), f.value = l.selectionText, f.select();
+                    }), i.rightClickHandler = i.moveTextAreaUnderMouseCursor = i.paste = i.handlePasteEvent = i.copyHandler = i.bracketTextForPaste = i.prepareTextForTerminal = void 0, i.prepareTextForTerminal = n, i.bracketTextForPaste = o, i.copyHandler = function(d, v) {
+                        d.clipboardData && d.clipboardData.setData("text/plain", v.selectionText), d.preventDefault();
+                    }, i.handlePasteEvent = function(d, v, m, l) {
+                        d.stopPropagation(), d.clipboardData && c(d.clipboardData.getData("text/plain"), v, m, l);
+                    }, i.paste = c, i.moveTextAreaUnderMouseCursor = a, i.rightClickHandler = function(d, v, m, l, s) {
+                        a(d, v, m), s && l.rightClickSelect(d), v.value = l.selectionText, v.select();
                     };
                 },
                 7239: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.ColorContrastCache = void 0;
                     const o = n(1505);
@@ -2507,336 +2507,336 @@
                             dispose: () => {
                                 d || (d = !0, n.removeEventListener(o, c, a));
                             }
                         };
                     };
                 },
                 3551: function(k, i, n) {
-                    var o = this && this.__decorate || function(r, t, e, h) {
-                            var v, u = arguments.length,
-                                p = u < 3 ? t : h === null ? h = Object.getOwnPropertyDescriptor(t, e) : h;
+                    var o = this && this.__decorate || function(r, e, t, h) {
+                            var g, u = arguments.length,
+                                S = u < 3 ? e : h === null ? h = Object.getOwnPropertyDescriptor(e, t) : h;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                p = Reflect.decorate(r, t, e, h);
+                                S = Reflect.decorate(r, e, t, h);
                             else
                                 for (var _ = r.length - 1; _ >= 0; _--)
-                                    (v = r[_]) && (p = (u < 3 ? v(p) : u > 3 ? v(t, e, p) : v(t, e)) || p);
-                            return u > 3 && p && Object.defineProperty(t, e, p), p;
+                                    (g = r[_]) && (S = (u < 3 ? g(S) : u > 3 ? g(e, t, S) : g(e, t)) || S);
+                            return u > 3 && S && Object.defineProperty(e, t, S), S;
                         },
-                        c = this && this.__param || function(r, t) {
-                            return function(e, h) {
-                                t(e, h, r);
+                        c = this && this.__param || function(r, e) {
+                            return function(t, h) {
+                                e(t, h, r);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.Linkifier = void 0;
                     const a = n(3656),
                         d = n(8460),
-                        f = n(844),
-                        g = n(2585),
+                        v = n(844),
+                        m = n(2585),
                         l = n(4725);
-                    let s = i.Linkifier = class extends f.Disposable {
+                    let s = i.Linkifier = class extends v.Disposable {
                         get currentLink() {
                             return this._currentLink;
                         }
-                        constructor(r, t, e, h, v) {
-                            super(), this._element = r, this._mouseService = t, this._renderService = e, this._bufferService = h, this._linkProviderService = v, this._linkCacheDisposables = [], this._isMouseOut = !0, this._wasResized = !1, this._activeLine = -1, this._onShowLinkUnderline = this.register(new d.EventEmitter()), this.onShowLinkUnderline = this._onShowLinkUnderline.event, this._onHideLinkUnderline = this.register(new d.EventEmitter()), this.onHideLinkUnderline = this._onHideLinkUnderline.event, this.register((0, f.getDisposeArrayDisposable)(this._linkCacheDisposables)), this.register((0, f.toDisposable)(() => {
+                        constructor(r, e, t, h, g) {
+                            super(), this._element = r, this._mouseService = e, this._renderService = t, this._bufferService = h, this._linkProviderService = g, this._linkCacheDisposables = [], this._isMouseOut = !0, this._wasResized = !1, this._activeLine = -1, this._onShowLinkUnderline = this.register(new d.EventEmitter()), this.onShowLinkUnderline = this._onShowLinkUnderline.event, this._onHideLinkUnderline = this.register(new d.EventEmitter()), this.onHideLinkUnderline = this._onHideLinkUnderline.event, this.register((0, v.getDisposeArrayDisposable)(this._linkCacheDisposables)), this.register((0, v.toDisposable)(() => {
                                 var u;
                                 this._lastMouseEvent = void 0, (u = this._activeProviderReplies) == null || u.clear();
                             })), this.register(this._bufferService.onResize(() => {
                                 this._clearCurrentLink(), this._wasResized = !0;
                             })), this.register((0, a.addDisposableDomListener)(this._element, "mouseleave", () => {
                                 this._isMouseOut = !0, this._clearCurrentLink();
                             })), this.register((0, a.addDisposableDomListener)(this._element, "mousemove", this._handleMouseMove.bind(this))), this.register((0, a.addDisposableDomListener)(this._element, "mousedown", this._handleMouseDown.bind(this))), this.register((0, a.addDisposableDomListener)(this._element, "mouseup", this._handleMouseUp.bind(this)));
                         }
                         _handleMouseMove(r) {
                             this._lastMouseEvent = r;
-                            const t = this._positionFromMouseEvent(r, this._element, this._mouseService);
-                            if (!t)
+                            const e = this._positionFromMouseEvent(r, this._element, this._mouseService);
+                            if (!e)
                                 return;
                             this._isMouseOut = !1;
-                            const e = r.composedPath();
-                            for (let h = 0; h < e.length; h++) {
-                                const v = e[h];
-                                if (v.classList.contains("xterm"))
+                            const t = r.composedPath();
+                            for (let h = 0; h < t.length; h++) {
+                                const g = t[h];
+                                if (g.classList.contains("xterm"))
                                     break;
-                                if (v.classList.contains("xterm-hover"))
+                                if (g.classList.contains("xterm-hover"))
                                     return;
                             }
-                            this._lastBufferCell && t.x === this._lastBufferCell.x && t.y === this._lastBufferCell.y || (this._handleHover(t), this._lastBufferCell = t);
+                            this._lastBufferCell && e.x === this._lastBufferCell.x && e.y === this._lastBufferCell.y || (this._handleHover(e), this._lastBufferCell = e);
                         }
                         _handleHover(r) {
                             if (this._activeLine !== r.y || this._wasResized)
                                 return this._clearCurrentLink(), this._askForLink(r, !1), void(this._wasResized = !1);
                             this._currentLink && this._linkAtPosition(this._currentLink.link, r) || (this._clearCurrentLink(), this._askForLink(r, !0));
                         }
-                        _askForLink(r, t) {
-                            var h, v;
-                            this._activeProviderReplies && t || ((h = this._activeProviderReplies) == null || h.forEach((u) => {
-                                u == null || u.forEach((p) => {
-                                    p.link.dispose && p.link.dispose();
+                        _askForLink(r, e) {
+                            var h, g;
+                            this._activeProviderReplies && e || ((h = this._activeProviderReplies) == null || h.forEach((u) => {
+                                u == null || u.forEach((S) => {
+                                    S.link.dispose && S.link.dispose();
                                 });
                             }), this._activeProviderReplies = /* @__PURE__ */ new Map(), this._activeLine = r.y);
-                            let e = !1;
-                            for (const [u, p] of this._linkProviderService.linkProviders.entries())
-                                t ? (v = this._activeProviderReplies) != null && v.get(u) && (e = this._checkLinkProviderResult(u, r, e)) : p.provideLinks(r.y, (_) => {
-                                    var A, T;
+                            let t = !1;
+                            for (const [u, S] of this._linkProviderService.linkProviders.entries())
+                                e ? (g = this._activeProviderReplies) != null && g.get(u) && (t = this._checkLinkProviderResult(u, r, t)) : S.provideLinks(r.y, (_) => {
+                                    var R, B;
                                     if (this._isMouseOut)
                                         return;
-                                    const b = _ == null ? void 0 : _.map((x) => ({
-                                        link: x
+                                    const b = _ == null ? void 0 : _.map((T) => ({
+                                        link: T
                                     }));
-                                    (A = this._activeProviderReplies) == null || A.set(u, b), e = this._checkLinkProviderResult(u, r, e), ((T = this._activeProviderReplies) == null ? void 0 : T.size) === this._linkProviderService.linkProviders.length && this._removeIntersectingLinks(r.y, this._activeProviderReplies);
+                                    (R = this._activeProviderReplies) == null || R.set(u, b), t = this._checkLinkProviderResult(u, r, t), ((B = this._activeProviderReplies) == null ? void 0 : B.size) === this._linkProviderService.linkProviders.length && this._removeIntersectingLinks(r.y, this._activeProviderReplies);
                                 });
                         }
-                        _removeIntersectingLinks(r, t) {
-                            const e = /* @__PURE__ */ new Set();
-                            for (let h = 0; h < t.size; h++) {
-                                const v = t.get(h);
-                                if (v)
-                                    for (let u = 0; u < v.length; u++) {
-                                        const p = v[u],
-                                            _ = p.link.range.start.y < r ? 0 : p.link.range.start.x,
-                                            b = p.link.range.end.y > r ? this._bufferService.cols : p.link.range.end.x;
-                                        for (let A = _; A <= b; A++) {
-                                            if (e.has(A)) {
-                                                v.splice(u--, 1);
+                        _removeIntersectingLinks(r, e) {
+                            const t = /* @__PURE__ */ new Set();
+                            for (let h = 0; h < e.size; h++) {
+                                const g = e.get(h);
+                                if (g)
+                                    for (let u = 0; u < g.length; u++) {
+                                        const S = g[u],
+                                            _ = S.link.range.start.y < r ? 0 : S.link.range.start.x,
+                                            b = S.link.range.end.y > r ? this._bufferService.cols : S.link.range.end.x;
+                                        for (let R = _; R <= b; R++) {
+                                            if (t.has(R)) {
+                                                g.splice(u--, 1);
                                                 break;
                                             }
-                                            e.add(A);
+                                            t.add(R);
                                         }
                                     }
                             }
                         }
-                        _checkLinkProviderResult(r, t, e) {
+                        _checkLinkProviderResult(r, e, t) {
                             var u;
                             if (!this._activeProviderReplies)
-                                return e;
+                                return t;
                             const h = this._activeProviderReplies.get(r);
-                            let v = !1;
-                            for (let p = 0; p < r; p++)
-                                this._activeProviderReplies.has(p) && !this._activeProviderReplies.get(p) || (v = !0);
-                            if (!v && h) {
-                                const p = h.find((_) => this._linkAtPosition(_.link, t));
-                                p && (e = !0, this._handleNewLink(p));
-                            }
-                            if (this._activeProviderReplies.size === this._linkProviderService.linkProviders.length && !e)
-                                for (let p = 0; p < this._activeProviderReplies.size; p++) {
-                                    const _ = (u = this._activeProviderReplies.get(p)) == null ? void 0 : u.find((b) => this._linkAtPosition(b.link, t));
+                            let g = !1;
+                            for (let S = 0; S < r; S++)
+                                this._activeProviderReplies.has(S) && !this._activeProviderReplies.get(S) || (g = !0);
+                            if (!g && h) {
+                                const S = h.find((_) => this._linkAtPosition(_.link, e));
+                                S && (t = !0, this._handleNewLink(S));
+                            }
+                            if (this._activeProviderReplies.size === this._linkProviderService.linkProviders.length && !t)
+                                for (let S = 0; S < this._activeProviderReplies.size; S++) {
+                                    const _ = (u = this._activeProviderReplies.get(S)) == null ? void 0 : u.find((b) => this._linkAtPosition(b.link, e));
                                     if (_) {
-                                        e = !0, this._handleNewLink(_);
+                                        t = !0, this._handleNewLink(_);
                                         break;
                                     }
                                 }
-                            return e;
+                            return t;
                         }
                         _handleMouseDown() {
                             this._mouseDownLink = this._currentLink;
                         }
                         _handleMouseUp(r) {
                             if (!this._currentLink)
                                 return;
-                            const t = this._positionFromMouseEvent(r, this._element, this._mouseService);
-                            t && this._mouseDownLink === this._currentLink && this._linkAtPosition(this._currentLink.link, t) && this._currentLink.link.activate(r, this._currentLink.link.text);
+                            const e = this._positionFromMouseEvent(r, this._element, this._mouseService);
+                            e && this._mouseDownLink === this._currentLink && this._linkAtPosition(this._currentLink.link, e) && this._currentLink.link.activate(r, this._currentLink.link.text);
                         }
-                        _clearCurrentLink(r, t) {
-                            this._currentLink && this._lastMouseEvent && (!r || !t || this._currentLink.link.range.start.y >= r && this._currentLink.link.range.end.y <= t) && (this._linkLeave(this._element, this._currentLink.link, this._lastMouseEvent), this._currentLink = void 0, (0, f.disposeArray)(this._linkCacheDisposables));
+                        _clearCurrentLink(r, e) {
+                            this._currentLink && this._lastMouseEvent && (!r || !e || this._currentLink.link.range.start.y >= r && this._currentLink.link.range.end.y <= e) && (this._linkLeave(this._element, this._currentLink.link, this._lastMouseEvent), this._currentLink = void 0, (0, v.disposeArray)(this._linkCacheDisposables));
                         }
                         _handleNewLink(r) {
                             if (!this._lastMouseEvent)
                                 return;
-                            const t = this._positionFromMouseEvent(this._lastMouseEvent, this._element, this._mouseService);
-                            t && this._linkAtPosition(r.link, t) && (this._currentLink = r, this._currentLink.state = {
+                            const e = this._positionFromMouseEvent(this._lastMouseEvent, this._element, this._mouseService);
+                            e && this._linkAtPosition(r.link, e) && (this._currentLink = r, this._currentLink.state = {
                                 decorations: {
                                     underline: r.link.decorations === void 0 || r.link.decorations.underline,
                                     pointerCursor: r.link.decorations === void 0 || r.link.decorations.pointerCursor
                                 },
                                 isHovered: !0
                             }, this._linkHover(this._element, r.link, this._lastMouseEvent), r.link.decorations = {}, Object.defineProperties(r.link.decorations, {
                                 pointerCursor: {
                                     get: () => {
-                                        var e, h;
-                                        return (h = (e = this._currentLink) == null ? void 0 : e.state) == null ? void 0 : h.decorations.pointerCursor;
+                                        var t, h;
+                                        return (h = (t = this._currentLink) == null ? void 0 : t.state) == null ? void 0 : h.decorations.pointerCursor;
                                     },
-                                    set: (e) => {
+                                    set: (t) => {
                                         var h;
-                                        (h = this._currentLink) != null && h.state && this._currentLink.state.decorations.pointerCursor !== e && (this._currentLink.state.decorations.pointerCursor = e, this._currentLink.state.isHovered && this._element.classList.toggle("xterm-cursor-pointer", e));
+                                        (h = this._currentLink) != null && h.state && this._currentLink.state.decorations.pointerCursor !== t && (this._currentLink.state.decorations.pointerCursor = t, this._currentLink.state.isHovered && this._element.classList.toggle("xterm-cursor-pointer", t));
                                     }
                                 },
                                 underline: {
                                     get: () => {
-                                        var e, h;
-                                        return (h = (e = this._currentLink) == null ? void 0 : e.state) == null ? void 0 : h.decorations.underline;
+                                        var t, h;
+                                        return (h = (t = this._currentLink) == null ? void 0 : t.state) == null ? void 0 : h.decorations.underline;
                                     },
-                                    set: (e) => {
-                                        var h, v, u;
-                                        (h = this._currentLink) != null && h.state && ((u = (v = this._currentLink) == null ? void 0 : v.state) == null ? void 0 : u.decorations.underline) !== e && (this._currentLink.state.decorations.underline = e, this._currentLink.state.isHovered && this._fireUnderlineEvent(r.link, e));
+                                    set: (t) => {
+                                        var h, g, u;
+                                        (h = this._currentLink) != null && h.state && ((u = (g = this._currentLink) == null ? void 0 : g.state) == null ? void 0 : u.decorations.underline) !== t && (this._currentLink.state.decorations.underline = t, this._currentLink.state.isHovered && this._fireUnderlineEvent(r.link, t));
                                     }
                                 }
-                            }), this._linkCacheDisposables.push(this._renderService.onRenderedViewportChange((e) => {
+                            }), this._linkCacheDisposables.push(this._renderService.onRenderedViewportChange((t) => {
                                 if (!this._currentLink)
                                     return;
-                                const h = e.start === 0 ? 0 : e.start + 1 + this._bufferService.buffer.ydisp,
-                                    v = this._bufferService.buffer.ydisp + 1 + e.end;
-                                if (this._currentLink.link.range.start.y >= h && this._currentLink.link.range.end.y <= v && (this._clearCurrentLink(h, v), this._lastMouseEvent)) {
+                                const h = t.start === 0 ? 0 : t.start + 1 + this._bufferService.buffer.ydisp,
+                                    g = this._bufferService.buffer.ydisp + 1 + t.end;
+                                if (this._currentLink.link.range.start.y >= h && this._currentLink.link.range.end.y <= g && (this._clearCurrentLink(h, g), this._lastMouseEvent)) {
                                     const u = this._positionFromMouseEvent(this._lastMouseEvent, this._element, this._mouseService);
                                     u && this._askForLink(u, !1);
                                 }
                             })));
                         }
-                        _linkHover(r, t, e) {
+                        _linkHover(r, e, t) {
                             var h;
-                            (h = this._currentLink) != null && h.state && (this._currentLink.state.isHovered = !0, this._currentLink.state.decorations.underline && this._fireUnderlineEvent(t, !0), this._currentLink.state.decorations.pointerCursor && r.classList.add("xterm-cursor-pointer")), t.hover && t.hover(e, t.text);
+                            (h = this._currentLink) != null && h.state && (this._currentLink.state.isHovered = !0, this._currentLink.state.decorations.underline && this._fireUnderlineEvent(e, !0), this._currentLink.state.decorations.pointerCursor && r.classList.add("xterm-cursor-pointer")), e.hover && e.hover(t, e.text);
                         }
-                        _fireUnderlineEvent(r, t) {
-                            const e = r.range,
+                        _fireUnderlineEvent(r, e) {
+                            const t = r.range,
                                 h = this._bufferService.buffer.ydisp,
-                                v = this._createLinkUnderlineEvent(e.start.x - 1, e.start.y - h - 1, e.end.x, e.end.y - h - 1, void 0);
-                            (t ? this._onShowLinkUnderline : this._onHideLinkUnderline).fire(v);
+                                g = this._createLinkUnderlineEvent(t.start.x - 1, t.start.y - h - 1, t.end.x, t.end.y - h - 1, void 0);
+                            (e ? this._onShowLinkUnderline : this._onHideLinkUnderline).fire(g);
                         }
-                        _linkLeave(r, t, e) {
+                        _linkLeave(r, e, t) {
                             var h;
-                            (h = this._currentLink) != null && h.state && (this._currentLink.state.isHovered = !1, this._currentLink.state.decorations.underline && this._fireUnderlineEvent(t, !1), this._currentLink.state.decorations.pointerCursor && r.classList.remove("xterm-cursor-pointer")), t.leave && t.leave(e, t.text);
+                            (h = this._currentLink) != null && h.state && (this._currentLink.state.isHovered = !1, this._currentLink.state.decorations.underline && this._fireUnderlineEvent(e, !1), this._currentLink.state.decorations.pointerCursor && r.classList.remove("xterm-cursor-pointer")), e.leave && e.leave(t, e.text);
                         }
-                        _linkAtPosition(r, t) {
-                            const e = r.range.start.y * this._bufferService.cols + r.range.start.x,
+                        _linkAtPosition(r, e) {
+                            const t = r.range.start.y * this._bufferService.cols + r.range.start.x,
                                 h = r.range.end.y * this._bufferService.cols + r.range.end.x,
-                                v = t.y * this._bufferService.cols + t.x;
-                            return e <= v && v <= h;
+                                g = e.y * this._bufferService.cols + e.x;
+                            return t <= g && g <= h;
                         }
-                        _positionFromMouseEvent(r, t, e) {
-                            const h = e.getCoords(r, t, this._bufferService.cols, this._bufferService.rows);
+                        _positionFromMouseEvent(r, e, t) {
+                            const h = t.getCoords(r, e, this._bufferService.cols, this._bufferService.rows);
                             if (h)
                                 return {
                                     x: h[0],
                                     y: h[1] + this._bufferService.buffer.ydisp
                                 };
                         }
-                        _createLinkUnderlineEvent(r, t, e, h, v) {
+                        _createLinkUnderlineEvent(r, e, t, h, g) {
                             return {
                                 x1: r,
-                                y1: t,
-                                x2: e,
+                                y1: e,
+                                x2: t,
                                 y2: h,
                                 cols: this._bufferService.cols,
-                                fg: v
+                                fg: g
                             };
                         }
                     };
-                    i.Linkifier = s = o([c(1, l.IMouseService), c(2, l.IRenderService), c(3, g.IBufferService), c(4, l.ILinkProviderService)], s);
+                    i.Linkifier = s = o([c(1, l.IMouseService), c(2, l.IRenderService), c(3, m.IBufferService), c(4, l.ILinkProviderService)], s);
                 },
                 9042: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.tooMuchOutput = i.promptLabel = void 0, i.promptLabel = "Terminal input", i.tooMuchOutput = "Too much output to announce, navigate to rows manually to read";
                 },
                 3730: function(k, i, n) {
-                    var o = this && this.__decorate || function(l, s, r, t) {
-                            var e, h = arguments.length,
-                                v = h < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, r) : t;
+                    var o = this && this.__decorate || function(l, s, r, e) {
+                            var t, h = arguments.length,
+                                g = h < 3 ? s : e === null ? e = Object.getOwnPropertyDescriptor(s, r) : e;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                v = Reflect.decorate(l, s, r, t);
+                                g = Reflect.decorate(l, s, r, e);
                             else
                                 for (var u = l.length - 1; u >= 0; u--)
-                                    (e = l[u]) && (v = (h < 3 ? e(v) : h > 3 ? e(s, r, v) : e(s, r)) || v);
-                            return h > 3 && v && Object.defineProperty(s, r, v), v;
+                                    (t = l[u]) && (g = (h < 3 ? t(g) : h > 3 ? t(s, r, g) : t(s, r)) || g);
+                            return h > 3 && g && Object.defineProperty(s, r, g), g;
                         },
                         c = this && this.__param || function(l, s) {
-                            return function(r, t) {
-                                s(r, t, l);
+                            return function(r, e) {
+                                s(r, e, l);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.OscLinkProvider = void 0;
                     const a = n(511),
                         d = n(2585);
-                    let f = i.OscLinkProvider = class {
+                    let v = i.OscLinkProvider = class {
                         constructor(l, s, r) {
                             this._bufferService = l, this._optionsService = s, this._oscLinkService = r;
                         }
                         provideLinks(l, s) {
                             var b;
                             const r = this._bufferService.buffer.lines.get(l - 1);
                             if (!r)
                                 return void s(void 0);
-                            const t = [],
-                                e = this._optionsService.rawOptions.linkHandler,
+                            const e = [],
+                                t = this._optionsService.rawOptions.linkHandler,
                                 h = new a.CellData(),
-                                v = r.getTrimmedLength();
+                                g = r.getTrimmedLength();
                             let u = -1,
-                                p = -1,
+                                S = -1,
                                 _ = !1;
-                            for (let A = 0; A < v; A++)
-                                if (p !== -1 || r.hasContent(A)) {
-                                    if (r.loadCell(A, h), h.hasExtendedAttrs() && h.extended.urlId) {
-                                        if (p === -1) {
-                                            p = A, u = h.extended.urlId;
+                            for (let R = 0; R < g; R++)
+                                if (S !== -1 || r.hasContent(R)) {
+                                    if (r.loadCell(R, h), h.hasExtendedAttrs() && h.extended.urlId) {
+                                        if (S === -1) {
+                                            S = R, u = h.extended.urlId;
                                             continue;
                                         }
                                         _ = h.extended.urlId !== u;
                                     } else
-                                        p !== -1 && (_ = !0);
-                                    if (_ || p !== -1 && A === v - 1) {
-                                        const T = (b = this._oscLinkService.getLinkData(u)) == null ? void 0 : b.uri;
-                                        if (T) {
-                                            const x = {
+                                        S !== -1 && (_ = !0);
+                                    if (_ || S !== -1 && R === g - 1) {
+                                        const B = (b = this._oscLinkService.getLinkData(u)) == null ? void 0 : b.uri;
+                                        if (B) {
+                                            const T = {
                                                 start: {
-                                                    x: p + 1,
+                                                    x: S + 1,
                                                     y: l
                                                 },
                                                 end: {
-                                                    x: A + (_ || A !== v - 1 ? 0 : 1),
+                                                    x: R + (_ || R !== g - 1 ? 0 : 1),
                                                     y: l
                                                 }
                                             };
                                             let L = !1;
-                                            if (!(e != null && e.allowNonHttpProtocols))
+                                            if (!(t != null && t.allowNonHttpProtocols))
                                                 try {
-                                                    const H = new URL(T);
+                                                    const H = new URL(B);
                                                     ["http:", "https:"].includes(H.protocol) || (L = !0);
                                                 } catch {
                                                     L = !0;
                                                 }
-                                            L || t.push({
-                                                text: T,
-                                                range: x,
-                                                activate: (H, W) => e ? e.activate(H, W, x) : g(0, W),
+                                            L || e.push({
+                                                text: B,
+                                                range: T,
+                                                activate: (H, W) => t ? t.activate(H, W, T) : m(0, W),
                                                 hover: (H, W) => {
-                                                    var U;
-                                                    return (U = e == null ? void 0 : e.hover) == null ? void 0 : U.call(e, H, W, x);
+                                                    var j;
+                                                    return (j = t == null ? void 0 : t.hover) == null ? void 0 : j.call(t, H, W, T);
                                                 },
                                                 leave: (H, W) => {
-                                                    var U;
-                                                    return (U = e == null ? void 0 : e.leave) == null ? void 0 : U.call(e, H, W, x);
+                                                    var j;
+                                                    return (j = t == null ? void 0 : t.leave) == null ? void 0 : j.call(t, H, W, T);
                                                 }
                                             });
                                         }
-                                        _ = !1, h.hasExtendedAttrs() && h.extended.urlId ? (p = A, u = h.extended.urlId) : (p = -1, u = -1);
+                                        _ = !1, h.hasExtendedAttrs() && h.extended.urlId ? (S = R, u = h.extended.urlId) : (S = -1, u = -1);
                                     }
                                 }
-                            s(t);
+                            s(e);
                         }
                     };
 
-                    function g(l, s) {
+                    function m(l, s) {
                         if (confirm(`Do you want to navigate to ${s}?
 
 WARNING: This link could potentially be dangerous`)) {
                             const r = window.open();
                             if (r) {
                                 try {
                                     r.opener = null;
                                 } catch {}
                                 r.location.href = s;
                             } else
                                 console.warn("Opening link blocked as opener could not be cleared");
                         }
                     }
-                    i.OscLinkProvider = f = o([c(0, d.IBufferService), c(1, d.IOptionsService), c(2, d.IOscLinkService)], f);
+                    i.OscLinkProvider = v = o([c(0, d.IBufferService), c(1, d.IOptionsService), c(2, d.IOscLinkService)], v);
                 },
                 6193: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.RenderDebouncer = void 0, i.RenderDebouncer = class {
                         constructor(n, o) {
                             this._renderCallback = n, this._coreBrowserService = o, this._refreshCallbacks = [];
@@ -2868,43 +2868,43 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.Terminal = void 0;
                     const o = n(3614),
                         c = n(3656),
                         a = n(3551),
                         d = n(9042),
-                        f = n(3730),
-                        g = n(1680),
+                        v = n(3730),
+                        m = n(1680),
                         l = n(3107),
                         s = n(5744),
                         r = n(2950),
-                        t = n(1296),
-                        e = n(428),
+                        e = n(1296),
+                        t = n(428),
                         h = n(4269),
-                        v = n(5114),
+                        g = n(5114),
                         u = n(8934),
-                        p = n(3230),
+                        S = n(3230),
                         _ = n(9312),
                         b = n(4725),
-                        A = n(6731),
-                        T = n(8055),
-                        x = n(8969),
+                        R = n(6731),
+                        B = n(8055),
+                        T = n(8969),
                         L = n(8460),
                         H = n(844),
                         W = n(6114),
-                        U = n(8437),
-                        K = n(2584),
-                        j = n(7399),
+                        j = n(8437),
+                        V = n(2584),
+                        z = n(7399),
                         C = n(5941),
-                        D = n(9074),
-                        B = n(2585),
+                        x = n(9074),
+                        A = n(2585),
                         O = n(5435),
                         I = n(4567),
-                        z = n(779);
-                    class G extends x.CoreTerminal {
+                        q = n(779);
+                    class X extends T.CoreTerminal {
                         get onFocus() {
                             return this._onFocus.event;
                         }
                         get onBlur() {
                             return this._onBlur.event;
                         }
                         get onA11yChar() {
@@ -2913,47 +2913,47 @@
                         get onA11yTab() {
                             return this._onA11yTabEmitter.event;
                         }
                         get onWillOpen() {
                             return this._onWillOpen.event;
                         }
                         constructor(P = {}) {
-                            super(P), this.browser = W, this._keyDownHandled = !1, this._keyDownSeen = !1, this._keyPressHandled = !1, this._unprocessedDeadKey = !1, this._accessibilityManager = this.register(new H.MutableDisposable()), this._onCursorMove = this.register(new L.EventEmitter()), this.onCursorMove = this._onCursorMove.event, this._onKey = this.register(new L.EventEmitter()), this.onKey = this._onKey.event, this._onRender = this.register(new L.EventEmitter()), this.onRender = this._onRender.event, this._onSelectionChange = this.register(new L.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onTitleChange = this.register(new L.EventEmitter()), this.onTitleChange = this._onTitleChange.event, this._onBell = this.register(new L.EventEmitter()), this.onBell = this._onBell.event, this._onFocus = this.register(new L.EventEmitter()), this._onBlur = this.register(new L.EventEmitter()), this._onA11yCharEmitter = this.register(new L.EventEmitter()), this._onA11yTabEmitter = this.register(new L.EventEmitter()), this._onWillOpen = this.register(new L.EventEmitter()), this._setup(), this._decorationService = this._instantiationService.createInstance(D.DecorationService), this._instantiationService.setService(B.IDecorationService, this._decorationService), this._linkProviderService = this._instantiationService.createInstance(z.LinkProviderService), this._instantiationService.setService(b.ILinkProviderService, this._linkProviderService), this._linkProviderService.registerLinkProvider(this._instantiationService.createInstance(f.OscLinkProvider)), this.register(this._inputHandler.onRequestBell(() => this._onBell.fire())), this.register(this._inputHandler.onRequestRefreshRows((w, N) => this.refresh(w, N))), this.register(this._inputHandler.onRequestSendFocus(() => this._reportFocus())), this.register(this._inputHandler.onRequestReset(() => this.reset())), this.register(this._inputHandler.onRequestWindowsOptionsReport((w) => this._reportWindowsOptions(w))), this.register(this._inputHandler.onColor((w) => this._handleColorEvent(w))), this.register((0, L.forwardEvent)(this._inputHandler.onCursorMove, this._onCursorMove)), this.register((0, L.forwardEvent)(this._inputHandler.onTitleChange, this._onTitleChange)), this.register((0, L.forwardEvent)(this._inputHandler.onA11yChar, this._onA11yCharEmitter)), this.register((0, L.forwardEvent)(this._inputHandler.onA11yTab, this._onA11yTabEmitter)), this.register(this._bufferService.onResize((w) => this._afterResize(w.cols, w.rows))), this.register((0, H.toDisposable)(() => {
-                                var w, N;
-                                this._customKeyEventHandler = void 0, (N = (w = this.element) == null ? void 0 : w.parentNode) == null || N.removeChild(this.element);
+                            super(P), this.browser = W, this._keyDownHandled = !1, this._keyDownSeen = !1, this._keyPressHandled = !1, this._unprocessedDeadKey = !1, this._accessibilityManager = this.register(new H.MutableDisposable()), this._onCursorMove = this.register(new L.EventEmitter()), this.onCursorMove = this._onCursorMove.event, this._onKey = this.register(new L.EventEmitter()), this.onKey = this._onKey.event, this._onRender = this.register(new L.EventEmitter()), this.onRender = this._onRender.event, this._onSelectionChange = this.register(new L.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onTitleChange = this.register(new L.EventEmitter()), this.onTitleChange = this._onTitleChange.event, this._onBell = this.register(new L.EventEmitter()), this.onBell = this._onBell.event, this._onFocus = this.register(new L.EventEmitter()), this._onBlur = this.register(new L.EventEmitter()), this._onA11yCharEmitter = this.register(new L.EventEmitter()), this._onA11yTabEmitter = this.register(new L.EventEmitter()), this._onWillOpen = this.register(new L.EventEmitter()), this._setup(), this._decorationService = this._instantiationService.createInstance(x.DecorationService), this._instantiationService.setService(A.IDecorationService, this._decorationService), this._linkProviderService = this._instantiationService.createInstance(q.LinkProviderService), this._instantiationService.setService(b.ILinkProviderService, this._linkProviderService), this._linkProviderService.registerLinkProvider(this._instantiationService.createInstance(v.OscLinkProvider)), this.register(this._inputHandler.onRequestBell(() => this._onBell.fire())), this.register(this._inputHandler.onRequestRefreshRows((w, U) => this.refresh(w, U))), this.register(this._inputHandler.onRequestSendFocus(() => this._reportFocus())), this.register(this._inputHandler.onRequestReset(() => this.reset())), this.register(this._inputHandler.onRequestWindowsOptionsReport((w) => this._reportWindowsOptions(w))), this.register(this._inputHandler.onColor((w) => this._handleColorEvent(w))), this.register((0, L.forwardEvent)(this._inputHandler.onCursorMove, this._onCursorMove)), this.register((0, L.forwardEvent)(this._inputHandler.onTitleChange, this._onTitleChange)), this.register((0, L.forwardEvent)(this._inputHandler.onA11yChar, this._onA11yCharEmitter)), this.register((0, L.forwardEvent)(this._inputHandler.onA11yTab, this._onA11yTabEmitter)), this.register(this._bufferService.onResize((w) => this._afterResize(w.cols, w.rows))), this.register((0, H.toDisposable)(() => {
+                                var w, U;
+                                this._customKeyEventHandler = void 0, (U = (w = this.element) == null ? void 0 : w.parentNode) == null || U.removeChild(this.element);
                             }));
                         }
                         _handleColorEvent(P) {
                             if (this._themeService)
                                 for (const w of P) {
-                                    let N, F = "";
+                                    let U, F = "";
                                     switch (w.index) {
                                         case 256:
-                                            N = "foreground", F = "10";
+                                            U = "foreground", F = "10";
                                             break;
                                         case 257:
-                                            N = "background", F = "11";
+                                            U = "background", F = "11";
                                             break;
                                         case 258:
-                                            N = "cursor", F = "12";
+                                            U = "cursor", F = "12";
                                             break;
                                         default:
-                                            N = "ansi", F = "4;" + w.index;
+                                            U = "ansi", F = "4;" + w.index;
                                     }
                                     switch (w.type) {
                                         case 0:
-                                            const V = T.color.toColorRGB(N === "ansi" ? this._themeService.colors.ansi[w.index] : this._themeService.colors[N]);
-                                            this.coreService.triggerDataEvent(`${K.C0.ESC}]${F};${(0, C.toRgbString)(V)}${K.C1_ESCAPED.ST}`);
+                                            const G = B.color.toColorRGB(U === "ansi" ? this._themeService.colors.ansi[w.index] : this._themeService.colors[U]);
+                                            this.coreService.triggerDataEvent(`${V.C0.ESC}]${F};${(0, C.toRgbString)(G)}${V.C1_ESCAPED.ST}`);
                                             break;
                                         case 1:
-                                            if (N === "ansi")
-                                                this._themeService.modifyColors((q) => q.ansi[w.index] = T.channels.toColor(...w.color));
+                                            if (U === "ansi")
+                                                this._themeService.modifyColors((K) => K.ansi[w.index] = B.channels.toColor(...w.color));
                                             else {
-                                                const q = N;
-                                                this._themeService.modifyColors((Z) => Z[q] = T.channels.toColor(...w.color));
+                                                const K = U;
+                                                this._themeService.modifyColors((ee) => ee[K] = B.channels.toColor(...w.color));
                                             }
                                             break;
                                         case 2:
                                             this._themeService.restoreColor(w.index);
                                     }
                                 }
                         }
@@ -2968,37 +2968,37 @@
                                 preventScroll: !0
                             });
                         }
                         _handleScreenReaderModeOptionChange(P) {
                             P ? !this._accessibilityManager.value && this._renderService && (this._accessibilityManager.value = this._instantiationService.createInstance(I.AccessibilityManager, this)) : this._accessibilityManager.clear();
                         }
                         _handleTextAreaFocus(P) {
-                            this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(K.C0.ESC + "[I"), this.element.classList.add("focus"), this._showCursor(), this._onFocus.fire();
+                            this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(V.C0.ESC + "[I"), this.element.classList.add("focus"), this._showCursor(), this._onFocus.fire();
                         }
                         blur() {
                             var P;
                             return (P = this.textarea) == null ? void 0 : P.blur();
                         }
                         _handleTextAreaBlur() {
-                            this.textarea.value = "", this.refresh(this.buffer.y, this.buffer.y), this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(K.C0.ESC + "[O"), this.element.classList.remove("focus"), this._onBlur.fire();
+                            this.textarea.value = "", this.refresh(this.buffer.y, this.buffer.y), this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(V.C0.ESC + "[O"), this.element.classList.remove("focus"), this._onBlur.fire();
                         }
                         _syncTextArea() {
                             if (!this.textarea || !this.buffer.isCursorInViewport || this._compositionHelper.isComposing || !this._renderService)
                                 return;
                             const P = this.buffer.ybase + this.buffer.y,
                                 w = this.buffer.lines.get(P);
                             if (!w)
                                 return;
-                            const N = Math.min(this.buffer.x, this.cols - 1),
+                            const U = Math.min(this.buffer.x, this.cols - 1),
                                 F = this._renderService.dimensions.css.cell.height,
-                                V = w.getWidth(N),
-                                q = this._renderService.dimensions.css.cell.width * V,
-                                Z = this.buffer.y * this._renderService.dimensions.css.cell.height,
-                                ie = N * this._renderService.dimensions.css.cell.width;
-                            this.textarea.style.left = ie + "px", this.textarea.style.top = Z + "px", this.textarea.style.width = q + "px", this.textarea.style.height = F + "px", this.textarea.style.lineHeight = F + "px", this.textarea.style.zIndex = "-5";
+                                G = w.getWidth(U),
+                                K = this._renderService.dimensions.css.cell.width * G,
+                                ee = this.buffer.y * this._renderService.dimensions.css.cell.height,
+                                se = U * this._renderService.dimensions.css.cell.width;
+                            this.textarea.style.left = se + "px", this.textarea.style.top = ee + "px", this.textarea.style.width = K + "px", this.textarea.style.height = F + "px", this.textarea.style.lineHeight = F + "px", this.textarea.style.zIndex = "-5";
                         }
                         _initGlobal() {
                             this._bindKeys(), this.register((0, c.addDisposableDomListener)(this.element, "copy", (w) => {
                                 this.hasSelection() && (0, o.copyHandler)(w, this._selectionService);
                             }));
                             const P = (w) => (0, o.handlePasteEvent)(w, this.textarea, this.coreService, this.optionsService);
                             this.register((0, c.addDisposableDomListener)(this.textarea, "paste", P)), this.register((0, c.addDisposableDomListener)(this.element, "paste", P)), W.isFirefox ? this.register((0, c.addDisposableDomListener)(this.element, "mousedown", (w) => {
@@ -3009,144 +3009,144 @@
                                 w.button === 1 && (0, o.moveTextAreaUnderMouseCursor)(w, this.textarea, this.screenElement);
                             }));
                         }
                         _bindKeys() {
                             this.register((0, c.addDisposableDomListener)(this.textarea, "keyup", (P) => this._keyUp(P), !0)), this.register((0, c.addDisposableDomListener)(this.textarea, "keydown", (P) => this._keyDown(P), !0)), this.register((0, c.addDisposableDomListener)(this.textarea, "keypress", (P) => this._keyPress(P), !0)), this.register((0, c.addDisposableDomListener)(this.textarea, "compositionstart", () => this._compositionHelper.compositionstart())), this.register((0, c.addDisposableDomListener)(this.textarea, "compositionupdate", (P) => this._compositionHelper.compositionupdate(P))), this.register((0, c.addDisposableDomListener)(this.textarea, "compositionend", () => this._compositionHelper.compositionend())), this.register((0, c.addDisposableDomListener)(this.textarea, "input", (P) => this._inputEvent(P), !0)), this.register(this.onRender(() => this._compositionHelper.updateCompositionElements()));
                         }
                         open(P) {
-                            var N;
+                            var U;
                             if (!P)
                                 throw new Error("Terminal requires a parent element.");
-                            if (P.isConnected || this._logService.debug("Terminal.open was called on an element that was not attached to the DOM"), ((N = this.element) == null ? void 0 : N.ownerDocument.defaultView) && this._coreBrowserService)
+                            if (P.isConnected || this._logService.debug("Terminal.open was called on an element that was not attached to the DOM"), ((U = this.element) == null ? void 0 : U.ownerDocument.defaultView) && this._coreBrowserService)
                                 return void(this.element.ownerDocument.defaultView !== this._coreBrowserService.window && (this._coreBrowserService.window = this.element.ownerDocument.defaultView));
                             this._document = P.ownerDocument, this.options.documentOverride && this.options.documentOverride instanceof Document && (this._document = this.optionsService.rawOptions.documentOverride), this.element = this._document.createElement("div"), this.element.dir = "ltr", this.element.classList.add("terminal"), this.element.classList.add("xterm"), P.appendChild(this.element);
                             const w = this._document.createDocumentFragment();
-                            this._viewportElement = this._document.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), w.appendChild(this._viewportElement), this._viewportScrollArea = this._document.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = this._document.createElement("div"), this.screenElement.classList.add("xterm-screen"), this.register((0, c.addDisposableDomListener)(this.screenElement, "mousemove", (F) => this.updateCursorStyle(F))), this._helperContainer = this._document.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), w.appendChild(this.screenElement), this.textarea = this._document.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", d.promptLabel), W.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this.register(this._instantiationService.createInstance(v.CoreBrowserService, this.textarea, P.ownerDocument.defaultView ?? window, this._document ?? typeof window < "u" ? window.document : null)), this._instantiationService.setService(b.ICoreBrowserService, this._coreBrowserService), this.register((0, c.addDisposableDomListener)(this.textarea, "focus", (F) => this._handleTextAreaFocus(F))), this.register((0, c.addDisposableDomListener)(this.textarea, "blur", () => this._handleTextAreaBlur())), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(e.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(b.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance(A.ThemeService), this._instantiationService.setService(b.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(h.CharacterJoinerService), this._instantiationService.setService(b.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(p.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(b.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange((F) => this._onRender.fire(F))), this.onResize((F) => this._renderService.resize(F.cols, F.rows)), this._compositionView = this._document.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(r.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this._mouseService = this._instantiationService.createInstance(u.MouseService), this._instantiationService.setService(b.IMouseService, this._mouseService), this.linkifier = this.register(this._instantiationService.createInstance(a.Linkifier, this.screenElement)), this.element.appendChild(w);
+                            this._viewportElement = this._document.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), w.appendChild(this._viewportElement), this._viewportScrollArea = this._document.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = this._document.createElement("div"), this.screenElement.classList.add("xterm-screen"), this.register((0, c.addDisposableDomListener)(this.screenElement, "mousemove", (F) => this.updateCursorStyle(F))), this._helperContainer = this._document.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), w.appendChild(this.screenElement), this.textarea = this._document.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", d.promptLabel), W.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this.register(this._instantiationService.createInstance(g.CoreBrowserService, this.textarea, P.ownerDocument.defaultView ?? window, this._document ?? typeof window < "u" ? window.document : null)), this._instantiationService.setService(b.ICoreBrowserService, this._coreBrowserService), this.register((0, c.addDisposableDomListener)(this.textarea, "focus", (F) => this._handleTextAreaFocus(F))), this.register((0, c.addDisposableDomListener)(this.textarea, "blur", () => this._handleTextAreaBlur())), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(t.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(b.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance(R.ThemeService), this._instantiationService.setService(b.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(h.CharacterJoinerService), this._instantiationService.setService(b.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(S.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(b.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange((F) => this._onRender.fire(F))), this.onResize((F) => this._renderService.resize(F.cols, F.rows)), this._compositionView = this._document.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(r.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this._mouseService = this._instantiationService.createInstance(u.MouseService), this._instantiationService.setService(b.IMouseService, this._mouseService), this.linkifier = this.register(this._instantiationService.createInstance(a.Linkifier, this.screenElement)), this.element.appendChild(w);
                             try {
                                 this._onWillOpen.fire(this.element);
                             } catch {}
-                            this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this.viewport = this._instantiationService.createInstance(g.Viewport, this._viewportElement, this._viewportScrollArea), this.viewport.onRequestScrollLines((F) => this.scrollLines(F.amount, F.suppressScrollEvent, 1)), this.register(this._inputHandler.onRequestSyncScrollBar(() => this.viewport.syncScrollArea())), this.register(this.viewport), this.register(this.onCursorMove(() => {
+                            this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this.viewport = this._instantiationService.createInstance(m.Viewport, this._viewportElement, this._viewportScrollArea), this.viewport.onRequestScrollLines((F) => this.scrollLines(F.amount, F.suppressScrollEvent, 1)), this.register(this._inputHandler.onRequestSyncScrollBar(() => this.viewport.syncScrollArea())), this.register(this.viewport), this.register(this.onCursorMove(() => {
                                 this._renderService.handleCursorMove(), this._syncTextArea();
                             })), this.register(this.onResize(() => this._renderService.handleResize(this.cols, this.rows))), this.register(this.onBlur(() => this._renderService.handleBlur())), this.register(this.onFocus(() => this._renderService.handleFocus())), this.register(this._renderService.onDimensionsChange(() => this.viewport.syncScrollArea())), this._selectionService = this.register(this._instantiationService.createInstance(_.SelectionService, this.element, this.screenElement, this.linkifier)), this._instantiationService.setService(b.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines((F) => this.scrollLines(F.amount, F.suppressScrollEvent))), this.register(this._selectionService.onSelectionChange(() => this._onSelectionChange.fire())), this.register(this._selectionService.onRequestRedraw((F) => this._renderService.handleSelectionChanged(F.start, F.end, F.columnSelectMode))), this.register(this._selectionService.onLinuxMouseSelection((F) => {
                                 this.textarea.value = F, this.textarea.focus(), this.textarea.select();
                             })), this.register(this._onScroll.event((F) => {
                                 this.viewport.syncScrollArea(), this._selectionService.refresh();
                             })), this.register((0, c.addDisposableDomListener)(this._viewportElement, "scroll", () => this._selectionService.refresh())), this.register(this._instantiationService.createInstance(l.BufferDecorationRenderer, this.screenElement)), this.register((0, c.addDisposableDomListener)(this.element, "mousedown", (F) => this._selectionService.handleMouseDown(F))), this.coreMouseService.areMouseEventsActive ? (this._selectionService.disable(), this.element.classList.add("enable-mouse-events")) : this._selectionService.enable(), this.options.screenReaderMode && (this._accessibilityManager.value = this._instantiationService.createInstance(I.AccessibilityManager, this)), this.register(this.optionsService.onSpecificOptionChange("screenReaderMode", (F) => this._handleScreenReaderModeOptionChange(F))), this.options.overviewRulerWidth && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(s.OverviewRulerRenderer, this._viewportElement, this.screenElement))), this.optionsService.onSpecificOptionChange("overviewRulerWidth", (F) => {
                                 !this._overviewRulerRenderer && F && this._viewportElement && this.screenElement && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(s.OverviewRulerRenderer, this._viewportElement, this.screenElement)));
                             }), this._charSizeService.measure(), this.refresh(0, this.rows - 1), this._initGlobal(), this.bindMouse();
                         }
                         _createRenderer() {
-                            return this._instantiationService.createInstance(t.DomRenderer, this, this._document, this.element, this.screenElement, this._viewportElement, this._helperContainer, this.linkifier);
+                            return this._instantiationService.createInstance(e.DomRenderer, this, this._document, this.element, this.screenElement, this._viewportElement, this._helperContainer, this.linkifier);
                         }
                         bindMouse() {
                             const P = this,
                                 w = this.element;
 
-                            function N(q) {
-                                const Z = P._mouseService.getMouseReportCoords(q, P.screenElement);
-                                if (!Z)
+                            function U(K) {
+                                const ee = P._mouseService.getMouseReportCoords(K, P.screenElement);
+                                if (!ee)
                                     return !1;
-                                let ie, se;
-                                switch (q.overrideType || q.type) {
+                                let se, ie;
+                                switch (K.overrideType || K.type) {
                                     case "mousemove":
-                                        se = 32, q.buttons === void 0 ? (ie = 3, q.button !== void 0 && (ie = q.button < 3 ? q.button : 3)) : ie = 1 & q.buttons ? 0 : 4 & q.buttons ? 1 : 2 & q.buttons ? 2 : 3;
+                                        ie = 32, K.buttons === void 0 ? (se = 3, K.button !== void 0 && (se = K.button < 3 ? K.button : 3)) : se = 1 & K.buttons ? 0 : 4 & K.buttons ? 1 : 2 & K.buttons ? 2 : 3;
                                         break;
                                     case "mouseup":
-                                        se = 0, ie = q.button < 3 ? q.button : 3;
+                                        ie = 0, se = K.button < 3 ? K.button : 3;
                                         break;
                                     case "mousedown":
-                                        se = 1, ie = q.button < 3 ? q.button : 3;
+                                        ie = 1, se = K.button < 3 ? K.button : 3;
                                         break;
                                     case "wheel":
-                                        if (P._customWheelEventHandler && P._customWheelEventHandler(q) === !1 || P.viewport.getLinesScrolled(q) === 0)
+                                        if (P._customWheelEventHandler && P._customWheelEventHandler(K) === !1 || P.viewport.getLinesScrolled(K) === 0)
                                             return !1;
-                                        se = q.deltaY < 0 ? 0 : 1, ie = 4;
+                                        ie = K.deltaY < 0 ? 0 : 1, se = 4;
                                         break;
                                     default:
                                         return !1;
                                 }
-                                return !(se === void 0 || ie === void 0 || ie > 4) && P.coreMouseService.triggerMouseEvent({
-                                    col: Z.col,
-                                    row: Z.row,
-                                    x: Z.x,
-                                    y: Z.y,
-                                    button: ie,
-                                    action: se,
-                                    ctrl: q.ctrlKey,
-                                    alt: q.altKey,
-                                    shift: q.shiftKey
+                                return !(ie === void 0 || se === void 0 || se > 4) && P.coreMouseService.triggerMouseEvent({
+                                    col: ee.col,
+                                    row: ee.row,
+                                    x: ee.x,
+                                    y: ee.y,
+                                    button: se,
+                                    action: ie,
+                                    ctrl: K.ctrlKey,
+                                    alt: K.altKey,
+                                    shift: K.shiftKey
                                 });
                             }
                             const F = {
                                     mouseup: null,
                                     wheel: null,
                                     mousedrag: null,
                                     mousemove: null
                                 },
-                                V = {
-                                    mouseup: (q) => (N(q), q.buttons || (this._document.removeEventListener("mouseup", F.mouseup), F.mousedrag && this._document.removeEventListener("mousemove", F.mousedrag)), this.cancel(q)),
-                                    wheel: (q) => (N(q), this.cancel(q, !0)),
-                                    mousedrag: (q) => {
-                                        q.buttons && N(q);
+                                G = {
+                                    mouseup: (K) => (U(K), K.buttons || (this._document.removeEventListener("mouseup", F.mouseup), F.mousedrag && this._document.removeEventListener("mousemove", F.mousedrag)), this.cancel(K)),
+                                    wheel: (K) => (U(K), this.cancel(K, !0)),
+                                    mousedrag: (K) => {
+                                        K.buttons && U(K);
                                     },
-                                    mousemove: (q) => {
-                                        q.buttons || N(q);
+                                    mousemove: (K) => {
+                                        K.buttons || U(K);
                                     }
                                 };
-                            this.register(this.coreMouseService.onProtocolChange((q) => {
-                                q ? (this.optionsService.rawOptions.logLevel === "debug" && this._logService.debug("Binding to mouse events:", this.coreMouseService.explainEvents(q)), this.element.classList.add("enable-mouse-events"), this._selectionService.disable()) : (this._logService.debug("Unbinding from mouse events."), this.element.classList.remove("enable-mouse-events"), this._selectionService.enable()), 8 & q ? F.mousemove || (w.addEventListener("mousemove", V.mousemove), F.mousemove = V.mousemove) : (w.removeEventListener("mousemove", F.mousemove), F.mousemove = null), 16 & q ? F.wheel || (w.addEventListener("wheel", V.wheel, {
+                            this.register(this.coreMouseService.onProtocolChange((K) => {
+                                K ? (this.optionsService.rawOptions.logLevel === "debug" && this._logService.debug("Binding to mouse events:", this.coreMouseService.explainEvents(K)), this.element.classList.add("enable-mouse-events"), this._selectionService.disable()) : (this._logService.debug("Unbinding from mouse events."), this.element.classList.remove("enable-mouse-events"), this._selectionService.enable()), 8 & K ? F.mousemove || (w.addEventListener("mousemove", G.mousemove), F.mousemove = G.mousemove) : (w.removeEventListener("mousemove", F.mousemove), F.mousemove = null), 16 & K ? F.wheel || (w.addEventListener("wheel", G.wheel, {
                                     passive: !1
-                                }), F.wheel = V.wheel) : (w.removeEventListener("wheel", F.wheel), F.wheel = null), 2 & q ? F.mouseup || (F.mouseup = V.mouseup) : (this._document.removeEventListener("mouseup", F.mouseup), F.mouseup = null), 4 & q ? F.mousedrag || (F.mousedrag = V.mousedrag) : (this._document.removeEventListener("mousemove", F.mousedrag), F.mousedrag = null);
-                            })), this.coreMouseService.activeProtocol = this.coreMouseService.activeProtocol, this.register((0, c.addDisposableDomListener)(w, "mousedown", (q) => {
-                                if (q.preventDefault(), this.focus(), this.coreMouseService.areMouseEventsActive && !this._selectionService.shouldForceSelection(q))
-                                    return N(q), F.mouseup && this._document.addEventListener("mouseup", F.mouseup), F.mousedrag && this._document.addEventListener("mousemove", F.mousedrag), this.cancel(q);
-                            })), this.register((0, c.addDisposableDomListener)(w, "wheel", (q) => {
+                                }), F.wheel = G.wheel) : (w.removeEventListener("wheel", F.wheel), F.wheel = null), 2 & K ? F.mouseup || (F.mouseup = G.mouseup) : (this._document.removeEventListener("mouseup", F.mouseup), F.mouseup = null), 4 & K ? F.mousedrag || (F.mousedrag = G.mousedrag) : (this._document.removeEventListener("mousemove", F.mousedrag), F.mousedrag = null);
+                            })), this.coreMouseService.activeProtocol = this.coreMouseService.activeProtocol, this.register((0, c.addDisposableDomListener)(w, "mousedown", (K) => {
+                                if (K.preventDefault(), this.focus(), this.coreMouseService.areMouseEventsActive && !this._selectionService.shouldForceSelection(K))
+                                    return U(K), F.mouseup && this._document.addEventListener("mouseup", F.mouseup), F.mousedrag && this._document.addEventListener("mousemove", F.mousedrag), this.cancel(K);
+                            })), this.register((0, c.addDisposableDomListener)(w, "wheel", (K) => {
                                 if (!F.wheel) {
-                                    if (this._customWheelEventHandler && this._customWheelEventHandler(q) === !1)
+                                    if (this._customWheelEventHandler && this._customWheelEventHandler(K) === !1)
                                         return !1;
                                     if (!this.buffer.hasScrollback) {
-                                        const Z = this.viewport.getLinesScrolled(q);
-                                        if (Z === 0)
+                                        const ee = this.viewport.getLinesScrolled(K);
+                                        if (ee === 0)
                                             return;
-                                        const ie = K.C0.ESC + (this.coreService.decPrivateModes.applicationCursorKeys ? "O" : "[") + (q.deltaY < 0 ? "A" : "B");
-                                        let se = "";
-                                        for (let re = 0; re < Math.abs(Z); re++)
-                                            se += ie;
-                                        return this.coreService.triggerDataEvent(se, !0), this.cancel(q, !0);
+                                        const se = V.C0.ESC + (this.coreService.decPrivateModes.applicationCursorKeys ? "O" : "[") + (K.deltaY < 0 ? "A" : "B");
+                                        let ie = "";
+                                        for (let oe = 0; oe < Math.abs(ee); oe++)
+                                            ie += se;
+                                        return this.coreService.triggerDataEvent(ie, !0), this.cancel(K, !0);
                                     }
-                                    return this.viewport.handleWheel(q) ? this.cancel(q) : void 0;
+                                    return this.viewport.handleWheel(K) ? this.cancel(K) : void 0;
                                 }
                             }, {
                                 passive: !1
-                            })), this.register((0, c.addDisposableDomListener)(w, "touchstart", (q) => {
+                            })), this.register((0, c.addDisposableDomListener)(w, "touchstart", (K) => {
                                 if (!this.coreMouseService.areMouseEventsActive)
-                                    return this.viewport.handleTouchStart(q), this.cancel(q);
+                                    return this.viewport.handleTouchStart(K), this.cancel(K);
                             }, {
                                 passive: !0
-                            })), this.register((0, c.addDisposableDomListener)(w, "touchmove", (q) => {
+                            })), this.register((0, c.addDisposableDomListener)(w, "touchmove", (K) => {
                                 if (!this.coreMouseService.areMouseEventsActive)
-                                    return this.viewport.handleTouchMove(q) ? void 0 : this.cancel(q);
+                                    return this.viewport.handleTouchMove(K) ? void 0 : this.cancel(K);
                             }, {
                                 passive: !1
                             }));
                         }
                         refresh(P, w) {
-                            var N;
-                            (N = this._renderService) == null || N.refreshRows(P, w);
+                            var U;
+                            (U = this._renderService) == null || U.refreshRows(P, w);
                         }
                         updateCursorStyle(P) {
                             var w;
                             (w = this._selectionService) != null && w.shouldColumnSelect(P) ? this.element.classList.add("column-select") : this.element.classList.remove("column-select");
                         }
                         _showCursor() {
                             this.coreService.isCursorInitialized || (this.coreService.isCursorInitialized = !0, this.refresh(this.buffer.y, this.buffer.y));
                         }
-                        scrollLines(P, w, N = 0) {
+                        scrollLines(P, w, U = 0) {
                             var F;
-                            N === 1 ? (super.scrollLines(P, w, N), this.refresh(0, this.rows - 1)) : (F = this.viewport) == null || F.scrollLines(P);
+                            U === 1 ? (super.scrollLines(P, w, U), this.refresh(0, this.rows - 1)) : (F = this.viewport) == null || F.scrollLines(P);
                         }
                         paste(P) {
                             (0, o.paste)(P, this.textarea, this.coreService, this.optionsService);
                         }
                         attachCustomKeyEventHandler(P) {
                             this._customKeyEventHandler = P;
                         }
@@ -3175,16 +3175,16 @@
                         }
                         registerDecoration(P) {
                             return this._decorationService.registerDecoration(P);
                         }
                         hasSelection() {
                             return !!this._selectionService && this._selectionService.hasSelection;
                         }
-                        select(P, w, N) {
-                            this._selectionService.setSelection(P, w, N);
+                        select(P, w, U) {
+                            this._selectionService.setSelection(P, w, U);
                         }
                         getSelection() {
                             return this._selectionService ? this._selectionService.selectionText : "";
                         }
                         getSelectionPosition() {
                             if (this._selectionService && this._selectionService.hasSelection)
                                 return {
@@ -3203,37 +3203,37 @@
                             (P = this._selectionService) == null || P.clearSelection();
                         }
                         selectAll() {
                             var P;
                             (P = this._selectionService) == null || P.selectAll();
                         }
                         selectLines(P, w) {
-                            var N;
-                            (N = this._selectionService) == null || N.selectLines(P, w);
+                            var U;
+                            (U = this._selectionService) == null || U.selectLines(P, w);
                         }
                         _keyDown(P) {
                             if (this._keyDownHandled = !1, this._keyDownSeen = !0, this._customKeyEventHandler && this._customKeyEventHandler(P) === !1)
                                 return !1;
                             const w = this.browser.isMac && this.options.macOptionIsMeta && P.altKey;
                             if (!w && !this._compositionHelper.keydown(P))
                                 return this.options.scrollOnUserInput && this.buffer.ybase !== this.buffer.ydisp && this.scrollToBottom(), !1;
                             w || P.key !== "Dead" && P.key !== "AltGraph" || (this._unprocessedDeadKey = !0);
-                            const N = (0, j.evaluateKeyboardEvent)(P, this.coreService.decPrivateModes.applicationCursorKeys, this.browser.isMac, this.options.macOptionIsMeta);
-                            if (this.updateCursorStyle(P), N.type === 3 || N.type === 2) {
+                            const U = (0, z.evaluateKeyboardEvent)(P, this.coreService.decPrivateModes.applicationCursorKeys, this.browser.isMac, this.options.macOptionIsMeta);
+                            if (this.updateCursorStyle(P), U.type === 3 || U.type === 2) {
                                 const F = this.rows - 1;
-                                return this.scrollLines(N.type === 2 ? -F : F), this.cancel(P, !0);
+                                return this.scrollLines(U.type === 2 ? -F : F), this.cancel(P, !0);
                             }
-                            return N.type === 1 && this.selectAll(), !!this._isThirdLevelShift(this.browser, P) || (N.cancel && this.cancel(P, !0), !N.key || !!(P.key && !P.ctrlKey && !P.altKey && !P.metaKey && P.key.length === 1 && P.key.charCodeAt(0) >= 65 && P.key.charCodeAt(0) <= 90) || (this._unprocessedDeadKey ? (this._unprocessedDeadKey = !1, !0) : (N.key !== K.C0.ETX && N.key !== K.C0.CR || (this.textarea.value = ""), this._onKey.fire({
-                                key: N.key,
+                            return U.type === 1 && this.selectAll(), !!this._isThirdLevelShift(this.browser, P) || (U.cancel && this.cancel(P, !0), !U.key || !!(P.key && !P.ctrlKey && !P.altKey && !P.metaKey && P.key.length === 1 && P.key.charCodeAt(0) >= 65 && P.key.charCodeAt(0) <= 90) || (this._unprocessedDeadKey ? (this._unprocessedDeadKey = !1, !0) : (U.key !== V.C0.ETX && U.key !== V.C0.CR || (this.textarea.value = ""), this._onKey.fire({
+                                key: U.key,
                                 domEvent: P
-                            }), this._showCursor(), this.coreService.triggerDataEvent(N.key, !0), !this.optionsService.rawOptions.screenReaderMode || P.altKey || P.ctrlKey ? this.cancel(P, !0) : void(this._keyDownHandled = !0))));
+                            }), this._showCursor(), this.coreService.triggerDataEvent(U.key, !0), !this.optionsService.rawOptions.screenReaderMode || P.altKey || P.ctrlKey ? this.cancel(P, !0) : void(this._keyDownHandled = !0))));
                         }
                         _isThirdLevelShift(P, w) {
-                            const N = P.isMac && !this.options.macOptionIsMeta && w.altKey && !w.ctrlKey && !w.metaKey || P.isWindows && w.altKey && w.ctrlKey && !w.metaKey || P.isWindows && w.getModifierState("AltGraph");
-                            return w.type === "keypress" ? N : N && (!w.keyCode || w.keyCode > 47);
+                            const U = P.isMac && !this.options.macOptionIsMeta && w.altKey && !w.ctrlKey && !w.metaKey || P.isWindows && w.altKey && w.ctrlKey && !w.metaKey || P.isWindows && w.getModifierState("AltGraph");
+                            return w.type === "keypress" ? U : U && (!w.keyCode || w.keyCode > 47);
                         }
                         _keyUp(P) {
                             this._keyDownSeen = !1, this._customKeyEventHandler && this._customKeyEventHandler(P) === !1 || (function(w) {
                                 return w.keyCode === 16 || w.keyCode === 17 || w.keyCode === 18;
                             }(P) || this.focus(), this.updateCursorStyle(P), this._keyPressHandled = !1);
                         }
                         _keyPress(P) {
@@ -3264,63 +3264,63 @@
                             }
                             return !1;
                         }
                         resize(P, w) {
                             P !== this.cols || w !== this.rows ? super.resize(P, w) : this._charSizeService && !this._charSizeService.hasValidSize && this._charSizeService.measure();
                         }
                         _afterResize(P, w) {
-                            var N, F;
-                            (N = this._charSizeService) == null || N.measure(), (F = this.viewport) == null || F.syncScrollArea(!0);
+                            var U, F;
+                            (U = this._charSizeService) == null || U.measure(), (F = this.viewport) == null || F.syncScrollArea(!0);
                         }
                         clear() {
                             var P;
                             if (this.buffer.ybase !== 0 || this.buffer.y !== 0) {
                                 this.buffer.clearAllMarkers(), this.buffer.lines.set(0, this.buffer.lines.get(this.buffer.ybase + this.buffer.y)), this.buffer.lines.length = 1, this.buffer.ydisp = 0, this.buffer.ybase = 0, this.buffer.y = 0;
                                 for (let w = 1; w < this.rows; w++)
-                                    this.buffer.lines.push(this.buffer.getBlankLine(U.DEFAULT_ATTR_DATA));
+                                    this.buffer.lines.push(this.buffer.getBlankLine(j.DEFAULT_ATTR_DATA));
                                 this._onScroll.fire({
                                     position: this.buffer.ydisp,
                                     source: 0
                                 }), (P = this.viewport) == null || P.reset(), this.refresh(0, this.rows - 1);
                             }
                         }
                         reset() {
-                            var w, N;
+                            var w, U;
                             this.options.rows = this.rows, this.options.cols = this.cols;
                             const P = this._customKeyEventHandler;
-                            this._setup(), super.reset(), (w = this._selectionService) == null || w.reset(), this._decorationService.reset(), (N = this.viewport) == null || N.reset(), this._customKeyEventHandler = P, this.refresh(0, this.rows - 1);
+                            this._setup(), super.reset(), (w = this._selectionService) == null || w.reset(), this._decorationService.reset(), (U = this.viewport) == null || U.reset(), this._customKeyEventHandler = P, this.refresh(0, this.rows - 1);
                         }
                         clearTextureAtlas() {
                             var P;
                             (P = this._renderService) == null || P.clearTextureAtlas();
                         }
                         _reportFocus() {
                             var P;
-                            (P = this.element) != null && P.classList.contains("focus") ? this.coreService.triggerDataEvent(K.C0.ESC + "[I") : this.coreService.triggerDataEvent(K.C0.ESC + "[O");
+                            (P = this.element) != null && P.classList.contains("focus") ? this.coreService.triggerDataEvent(V.C0.ESC + "[I") : this.coreService.triggerDataEvent(V.C0.ESC + "[O");
                         }
                         _reportWindowsOptions(P) {
                             if (this._renderService)
                                 switch (P) {
                                     case O.WindowsOptionsReportType.GET_WIN_SIZE_PIXELS:
                                         const w = this._renderService.dimensions.css.canvas.width.toFixed(0),
-                                            N = this._renderService.dimensions.css.canvas.height.toFixed(0);
-                                        this.coreService.triggerDataEvent(`${K.C0.ESC}[4;${N};${w}t`);
+                                            U = this._renderService.dimensions.css.canvas.height.toFixed(0);
+                                        this.coreService.triggerDataEvent(`${V.C0.ESC}[4;${U};${w}t`);
                                         break;
                                     case O.WindowsOptionsReportType.GET_CELL_SIZE_PIXELS:
                                         const F = this._renderService.dimensions.css.cell.width.toFixed(0),
-                                            V = this._renderService.dimensions.css.cell.height.toFixed(0);
-                                        this.coreService.triggerDataEvent(`${K.C0.ESC}[6;${V};${F}t`);
+                                            G = this._renderService.dimensions.css.cell.height.toFixed(0);
+                                        this.coreService.triggerDataEvent(`${V.C0.ESC}[6;${G};${F}t`);
                                 }
                         }
                         cancel(P, w) {
                             if (this.options.cancelEvents || w)
                                 return P.preventDefault(), P.stopPropagation(), !1;
                         }
                     }
-                    i.Terminal = G;
+                    i.Terminal = X;
                 },
                 9924: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.TimeBasedDebouncer = void 0, i.TimeBasedDebouncer = class {
                         constructor(n, o = 1e3) {
                             this._renderCallback = n, this._debounceThresholdMS = o, this._lastRefreshMs = 0, this._additionalRefreshRequested = !1;
@@ -3331,60 +3331,60 @@
                         refresh(n, o, c) {
                             this._rowCount = c, n = n !== void 0 ? n : 0, o = o !== void 0 ? o : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, n) : n, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, o) : o;
                             const a = Date.now();
                             if (a - this._lastRefreshMs >= this._debounceThresholdMS)
                                 this._lastRefreshMs = a, this._innerRefresh();
                             else if (!this._additionalRefreshRequested) {
                                 const d = a - this._lastRefreshMs,
-                                    f = this._debounceThresholdMS - d;
+                                    v = this._debounceThresholdMS - d;
                                 this._additionalRefreshRequested = !0, this._refreshTimeoutID = window.setTimeout(() => {
                                     this._lastRefreshMs = Date.now(), this._innerRefresh(), this._additionalRefreshRequested = !1, this._refreshTimeoutID = void 0;
-                                }, f);
+                                }, v);
                             }
                         }
                         _innerRefresh() {
                             if (this._rowStart === void 0 || this._rowEnd === void 0 || this._rowCount === void 0)
                                 return;
                             const n = Math.max(this._rowStart, 0),
                                 o = Math.min(this._rowEnd, this._rowCount - 1);
                             this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(n, o);
                         }
                     };
                 },
                 1680: function(k, i, n) {
-                    var o = this && this.__decorate || function(r, t, e, h) {
-                            var v, u = arguments.length,
-                                p = u < 3 ? t : h === null ? h = Object.getOwnPropertyDescriptor(t, e) : h;
+                    var o = this && this.__decorate || function(r, e, t, h) {
+                            var g, u = arguments.length,
+                                S = u < 3 ? e : h === null ? h = Object.getOwnPropertyDescriptor(e, t) : h;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                p = Reflect.decorate(r, t, e, h);
+                                S = Reflect.decorate(r, e, t, h);
                             else
                                 for (var _ = r.length - 1; _ >= 0; _--)
-                                    (v = r[_]) && (p = (u < 3 ? v(p) : u > 3 ? v(t, e, p) : v(t, e)) || p);
-                            return u > 3 && p && Object.defineProperty(t, e, p), p;
+                                    (g = r[_]) && (S = (u < 3 ? g(S) : u > 3 ? g(e, t, S) : g(e, t)) || S);
+                            return u > 3 && S && Object.defineProperty(e, t, S), S;
                         },
-                        c = this && this.__param || function(r, t) {
-                            return function(e, h) {
-                                t(e, h, r);
+                        c = this && this.__param || function(r, e) {
+                            return function(t, h) {
+                                e(t, h, r);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.Viewport = void 0;
                     const a = n(3656),
                         d = n(4725),
-                        f = n(8460),
-                        g = n(844),
+                        v = n(8460),
+                        m = n(844),
                         l = n(2585);
-                    let s = i.Viewport = class extends g.Disposable {
-                        constructor(r, t, e, h, v, u, p, _) {
-                            super(), this._viewportElement = r, this._scrollArea = t, this._bufferService = e, this._optionsService = h, this._charSizeService = v, this._renderService = u, this._coreBrowserService = p, this.scrollBarWidth = 0, this._currentRowHeight = 0, this._currentDeviceCellHeight = 0, this._lastRecordedBufferLength = 0, this._lastRecordedViewportHeight = 0, this._lastRecordedBufferHeight = 0, this._lastTouchY = 0, this._lastScrollTop = 0, this._wheelPartialScroll = 0, this._refreshAnimationFrame = null, this._ignoreNextScrollEvent = !1, this._smoothScrollState = {
+                    let s = i.Viewport = class extends m.Disposable {
+                        constructor(r, e, t, h, g, u, S, _) {
+                            super(), this._viewportElement = r, this._scrollArea = e, this._bufferService = t, this._optionsService = h, this._charSizeService = g, this._renderService = u, this._coreBrowserService = S, this.scrollBarWidth = 0, this._currentRowHeight = 0, this._currentDeviceCellHeight = 0, this._lastRecordedBufferLength = 0, this._lastRecordedViewportHeight = 0, this._lastRecordedBufferHeight = 0, this._lastTouchY = 0, this._lastScrollTop = 0, this._wheelPartialScroll = 0, this._refreshAnimationFrame = null, this._ignoreNextScrollEvent = !1, this._smoothScrollState = {
                                 startTime: 0,
                                 origin: -1,
                                 target: -1
-                            }, this._onRequestScrollLines = this.register(new f.EventEmitter()), this.onRequestScrollLines = this._onRequestScrollLines.event, this.scrollBarWidth = this._viewportElement.offsetWidth - this._scrollArea.offsetWidth || 15, this.register((0, a.addDisposableDomListener)(this._viewportElement, "scroll", this._handleScroll.bind(this))), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate((b) => this._activeBuffer = b.activeBuffer)), this._renderDimensions = this._renderService.dimensions, this.register(this._renderService.onDimensionsChange((b) => this._renderDimensions = b)), this._handleThemeChange(_.colors), this.register(_.onChangeColors((b) => this._handleThemeChange(b))), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.syncScrollArea())), setTimeout(() => this.syncScrollArea());
+                            }, this._onRequestScrollLines = this.register(new v.EventEmitter()), this.onRequestScrollLines = this._onRequestScrollLines.event, this.scrollBarWidth = this._viewportElement.offsetWidth - this._scrollArea.offsetWidth || 15, this.register((0, a.addDisposableDomListener)(this._viewportElement, "scroll", this._handleScroll.bind(this))), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate((b) => this._activeBuffer = b.activeBuffer)), this._renderDimensions = this._renderService.dimensions, this.register(this._renderService.onDimensionsChange((b) => this._renderDimensions = b)), this._handleThemeChange(_.colors), this.register(_.onChangeColors((b) => this._handleThemeChange(b))), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.syncScrollArea())), setTimeout(() => this.syncScrollArea());
                         }
                         _handleThemeChange(r) {
                             this._viewportElement.style.backgroundColor = r.background.css;
                         }
                         reset() {
                             this._currentRowHeight = 0, this._currentDeviceCellHeight = 0, this._lastRecordedBufferLength = 0, this._lastRecordedViewportHeight = 0, this._lastRecordedBufferHeight = 0, this._lastTouchY = 0, this._lastScrollTop = 0, this._coreBrowserService.window.requestAnimationFrame(() => this.syncScrollArea());
                         }
@@ -3392,16 +3392,16 @@
                             if (r)
                                 return this._innerRefresh(), void(this._refreshAnimationFrame !== null && this._coreBrowserService.window.cancelAnimationFrame(this._refreshAnimationFrame));
                             this._refreshAnimationFrame === null && (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame(() => this._innerRefresh()));
                         }
                         _innerRefresh() {
                             if (this._charSizeService.height > 0) {
                                 this._currentRowHeight = this._renderDimensions.device.cell.height / this._coreBrowserService.dpr, this._currentDeviceCellHeight = this._renderDimensions.device.cell.height, this._lastRecordedViewportHeight = this._viewportElement.offsetHeight;
-                                const t = Math.round(this._currentRowHeight * this._lastRecordedBufferLength) + (this._lastRecordedViewportHeight - this._renderDimensions.css.canvas.height);
-                                this._lastRecordedBufferHeight !== t && (this._lastRecordedBufferHeight = t, this._scrollArea.style.height = this._lastRecordedBufferHeight + "px");
+                                const e = Math.round(this._currentRowHeight * this._lastRecordedBufferLength) + (this._lastRecordedViewportHeight - this._renderDimensions.css.canvas.height);
+                                this._lastRecordedBufferHeight !== e && (this._lastRecordedBufferHeight = e, this._scrollArea.style.height = this._lastRecordedBufferHeight + "px");
                             }
                             const r = this._bufferService.buffer.ydisp * this._currentRowHeight;
                             this._viewportElement.scrollTop !== r && (this._ignoreNextScrollEvent = !0, this._viewportElement.scrollTop = r), this._refreshAnimationFrame = null;
                         }
                         syncScrollArea(r = !1) {
                             if (this._lastRecordedBufferLength !== this._bufferService.buffer.lines.length)
                                 return this._lastRecordedBufferLength = this._bufferService.buffer.lines.length, void this._refresh(r);
@@ -3411,17 +3411,17 @@
                             if (this._lastScrollTop = this._viewportElement.scrollTop, !this._viewportElement.offsetParent)
                                 return;
                             if (this._ignoreNextScrollEvent)
                                 return this._ignoreNextScrollEvent = !1, void this._onRequestScrollLines.fire({
                                     amount: 0,
                                     suppressScrollEvent: !0
                                 });
-                            const t = Math.round(this._lastScrollTop / this._currentRowHeight) - this._bufferService.buffer.ydisp;
+                            const e = Math.round(this._lastScrollTop / this._currentRowHeight) - this._bufferService.buffer.ydisp;
                             this._onRequestScrollLines.fire({
-                                amount: t,
+                                amount: e,
                                 suppressScrollEvent: !0
                             });
                         }
                         _smoothScroll() {
                             if (this._isDisposed || this._smoothScrollState.origin === -1 || this._smoothScrollState.target === -1)
                                 return;
                             const r = this._smoothScrollPercent();
@@ -3429,105 +3429,105 @@
                         }
                         _smoothScrollPercent() {
                             return this._optionsService.rawOptions.smoothScrollDuration && this._smoothScrollState.startTime ? Math.max(Math.min((Date.now() - this._smoothScrollState.startTime) / this._optionsService.rawOptions.smoothScrollDuration, 1), 0) : 1;
                         }
                         _clearSmoothScrollState() {
                             this._smoothScrollState.startTime = 0, this._smoothScrollState.origin = -1, this._smoothScrollState.target = -1;
                         }
-                        _bubbleScroll(r, t) {
-                            const e = this._viewportElement.scrollTop + this._lastRecordedViewportHeight;
-                            return !(t < 0 && this._viewportElement.scrollTop !== 0 || t > 0 && e < this._lastRecordedBufferHeight) || (r.cancelable && r.preventDefault(), !1);
+                        _bubbleScroll(r, e) {
+                            const t = this._viewportElement.scrollTop + this._lastRecordedViewportHeight;
+                            return !(e < 0 && this._viewportElement.scrollTop !== 0 || e > 0 && t < this._lastRecordedBufferHeight) || (r.cancelable && r.preventDefault(), !1);
                         }
                         handleWheel(r) {
-                            const t = this._getPixelsScrolled(r);
-                            return t !== 0 && (this._optionsService.rawOptions.smoothScrollDuration ? (this._smoothScrollState.startTime = Date.now(), this._smoothScrollPercent() < 1 ? (this._smoothScrollState.origin = this._viewportElement.scrollTop, this._smoothScrollState.target === -1 ? this._smoothScrollState.target = this._viewportElement.scrollTop + t : this._smoothScrollState.target += t, this._smoothScrollState.target = Math.max(Math.min(this._smoothScrollState.target, this._viewportElement.scrollHeight), 0), this._smoothScroll()) : this._clearSmoothScrollState()) : this._viewportElement.scrollTop += t, this._bubbleScroll(r, t));
+                            const e = this._getPixelsScrolled(r);
+                            return e !== 0 && (this._optionsService.rawOptions.smoothScrollDuration ? (this._smoothScrollState.startTime = Date.now(), this._smoothScrollPercent() < 1 ? (this._smoothScrollState.origin = this._viewportElement.scrollTop, this._smoothScrollState.target === -1 ? this._smoothScrollState.target = this._viewportElement.scrollTop + e : this._smoothScrollState.target += e, this._smoothScrollState.target = Math.max(Math.min(this._smoothScrollState.target, this._viewportElement.scrollHeight), 0), this._smoothScroll()) : this._clearSmoothScrollState()) : this._viewportElement.scrollTop += e, this._bubbleScroll(r, e));
                         }
                         scrollLines(r) {
                             if (r !== 0)
                                 if (this._optionsService.rawOptions.smoothScrollDuration) {
-                                    const t = r * this._currentRowHeight;
-                                    this._smoothScrollState.startTime = Date.now(), this._smoothScrollPercent() < 1 ? (this._smoothScrollState.origin = this._viewportElement.scrollTop, this._smoothScrollState.target = this._smoothScrollState.origin + t, this._smoothScrollState.target = Math.max(Math.min(this._smoothScrollState.target, this._viewportElement.scrollHeight), 0), this._smoothScroll()) : this._clearSmoothScrollState();
+                                    const e = r * this._currentRowHeight;
+                                    this._smoothScrollState.startTime = Date.now(), this._smoothScrollPercent() < 1 ? (this._smoothScrollState.origin = this._viewportElement.scrollTop, this._smoothScrollState.target = this._smoothScrollState.origin + e, this._smoothScrollState.target = Math.max(Math.min(this._smoothScrollState.target, this._viewportElement.scrollHeight), 0), this._smoothScroll()) : this._clearSmoothScrollState();
                                 } else
                                     this._onRequestScrollLines.fire({
                                         amount: r,
                                         suppressScrollEvent: !1
                                     });
                         }
                         _getPixelsScrolled(r) {
                             if (r.deltaY === 0 || r.shiftKey)
                                 return 0;
-                            let t = this._applyScrollModifier(r.deltaY, r);
-                            return r.deltaMode === WheelEvent.DOM_DELTA_LINE ? t *= this._currentRowHeight : r.deltaMode === WheelEvent.DOM_DELTA_PAGE && (t *= this._currentRowHeight * this._bufferService.rows), t;
+                            let e = this._applyScrollModifier(r.deltaY, r);
+                            return r.deltaMode === WheelEvent.DOM_DELTA_LINE ? e *= this._currentRowHeight : r.deltaMode === WheelEvent.DOM_DELTA_PAGE && (e *= this._currentRowHeight * this._bufferService.rows), e;
                         }
-                        getBufferElements(r, t) {
+                        getBufferElements(r, e) {
                             var _;
-                            let e, h = "";
-                            const v = [],
-                                u = t ?? this._bufferService.buffer.lines.length,
-                                p = this._bufferService.buffer.lines;
+                            let t, h = "";
+                            const g = [],
+                                u = e ?? this._bufferService.buffer.lines.length,
+                                S = this._bufferService.buffer.lines;
                             for (let b = r; b < u; b++) {
-                                const A = p.get(b);
-                                if (!A)
+                                const R = S.get(b);
+                                if (!R)
                                     continue;
-                                const T = (_ = p.get(b + 1)) == null ? void 0 : _.isWrapped;
-                                if (h += A.translateToString(!T), !T || b === p.length - 1) {
-                                    const x = document.createElement("div");
-                                    x.textContent = h, v.push(x), h.length > 0 && (e = x), h = "";
+                                const B = (_ = S.get(b + 1)) == null ? void 0 : _.isWrapped;
+                                if (h += R.translateToString(!B), !B || b === S.length - 1) {
+                                    const T = document.createElement("div");
+                                    T.textContent = h, g.push(T), h.length > 0 && (t = T), h = "";
                                 }
                             }
                             return {
-                                bufferElements: v,
-                                cursorElement: e
+                                bufferElements: g,
+                                cursorElement: t
                             };
                         }
                         getLinesScrolled(r) {
                             if (r.deltaY === 0 || r.shiftKey)
                                 return 0;
-                            let t = this._applyScrollModifier(r.deltaY, r);
-                            return r.deltaMode === WheelEvent.DOM_DELTA_PIXEL ? (t /= this._currentRowHeight + 0, this._wheelPartialScroll += t, t = Math.floor(Math.abs(this._wheelPartialScroll)) * (this._wheelPartialScroll > 0 ? 1 : -1), this._wheelPartialScroll %= 1) : r.deltaMode === WheelEvent.DOM_DELTA_PAGE && (t *= this._bufferService.rows), t;
+                            let e = this._applyScrollModifier(r.deltaY, r);
+                            return r.deltaMode === WheelEvent.DOM_DELTA_PIXEL ? (e /= this._currentRowHeight + 0, this._wheelPartialScroll += e, e = Math.floor(Math.abs(this._wheelPartialScroll)) * (this._wheelPartialScroll > 0 ? 1 : -1), this._wheelPartialScroll %= 1) : r.deltaMode === WheelEvent.DOM_DELTA_PAGE && (e *= this._bufferService.rows), e;
                         }
-                        _applyScrollModifier(r, t) {
-                            const e = this._optionsService.rawOptions.fastScrollModifier;
-                            return e === "alt" && t.altKey || e === "ctrl" && t.ctrlKey || e === "shift" && t.shiftKey ? r * this._optionsService.rawOptions.fastScrollSensitivity * this._optionsService.rawOptions.scrollSensitivity : r * this._optionsService.rawOptions.scrollSensitivity;
+                        _applyScrollModifier(r, e) {
+                            const t = this._optionsService.rawOptions.fastScrollModifier;
+                            return t === "alt" && e.altKey || t === "ctrl" && e.ctrlKey || t === "shift" && e.shiftKey ? r * this._optionsService.rawOptions.fastScrollSensitivity * this._optionsService.rawOptions.scrollSensitivity : r * this._optionsService.rawOptions.scrollSensitivity;
                         }
                         handleTouchStart(r) {
                             this._lastTouchY = r.touches[0].pageY;
                         }
                         handleTouchMove(r) {
-                            const t = this._lastTouchY - r.touches[0].pageY;
-                            return this._lastTouchY = r.touches[0].pageY, t !== 0 && (this._viewportElement.scrollTop += t, this._bubbleScroll(r, t));
+                            const e = this._lastTouchY - r.touches[0].pageY;
+                            return this._lastTouchY = r.touches[0].pageY, e !== 0 && (this._viewportElement.scrollTop += e, this._bubbleScroll(r, e));
                         }
                     };
                     i.Viewport = s = o([c(2, l.IBufferService), c(3, l.IOptionsService), c(4, d.ICharSizeService), c(5, d.IRenderService), c(6, d.ICoreBrowserService), c(7, d.IThemeService)], s);
                 },
                 3107: function(k, i, n) {
-                    var o = this && this.__decorate || function(l, s, r, t) {
-                            var e, h = arguments.length,
-                                v = h < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, r) : t;
+                    var o = this && this.__decorate || function(l, s, r, e) {
+                            var t, h = arguments.length,
+                                g = h < 3 ? s : e === null ? e = Object.getOwnPropertyDescriptor(s, r) : e;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                v = Reflect.decorate(l, s, r, t);
+                                g = Reflect.decorate(l, s, r, e);
                             else
                                 for (var u = l.length - 1; u >= 0; u--)
-                                    (e = l[u]) && (v = (h < 3 ? e(v) : h > 3 ? e(s, r, v) : e(s, r)) || v);
-                            return h > 3 && v && Object.defineProperty(s, r, v), v;
+                                    (t = l[u]) && (g = (h < 3 ? t(g) : h > 3 ? t(s, r, g) : t(s, r)) || g);
+                            return h > 3 && g && Object.defineProperty(s, r, g), g;
                         },
                         c = this && this.__param || function(l, s) {
-                            return function(r, t) {
-                                s(r, t, l);
+                            return function(r, e) {
+                                s(r, e, l);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.BufferDecorationRenderer = void 0;
                     const a = n(4725),
                         d = n(844),
-                        f = n(2585);
-                    let g = i.BufferDecorationRenderer = class extends d.Disposable {
-                        constructor(l, s, r, t, e) {
-                            super(), this._screenElement = l, this._bufferService = s, this._coreBrowserService = r, this._decorationService = t, this._renderService = e, this._decorationElements = /* @__PURE__ */ new Map(), this._altBufferIsActive = !1, this._dimensionsChanged = !1, this._container = document.createElement("div"), this._container.classList.add("xterm-decoration-container"), this._screenElement.appendChild(this._container), this.register(this._renderService.onRenderedViewportChange(() => this._doRefreshDecorations())), this.register(this._renderService.onDimensionsChange(() => {
+                        v = n(2585);
+                    let m = i.BufferDecorationRenderer = class extends d.Disposable {
+                        constructor(l, s, r, e, t) {
+                            super(), this._screenElement = l, this._bufferService = s, this._coreBrowserService = r, this._decorationService = e, this._renderService = t, this._decorationElements = /* @__PURE__ */ new Map(), this._altBufferIsActive = !1, this._dimensionsChanged = !1, this._container = document.createElement("div"), this._container.classList.add("xterm-decoration-container"), this._screenElement.appendChild(this._container), this.register(this._renderService.onRenderedViewportChange(() => this._doRefreshDecorations())), this.register(this._renderService.onDimensionsChange(() => {
                                 this._dimensionsChanged = !0, this._queueRefresh();
                             })), this.register(this._coreBrowserService.onDprChange(() => this._queueRefresh())), this.register(this._bufferService.buffers.onBufferActivate(() => {
                                 this._altBufferIsActive = this._bufferService.buffer === this._bufferService.buffers.alt;
                             })), this.register(this._decorationService.onDecorationRegistered(() => this._queueRefresh())), this.register(this._decorationService.onDecorationRemoved((h) => this._removeDecoration(h))), this.register((0, d.toDisposable)(() => {
                                 this._container.remove(), this._decorationElements.clear();
                             }));
                         }
@@ -3541,17 +3541,17 @@
                                 this._renderDecoration(l);
                             this._dimensionsChanged = !1;
                         }
                         _renderDecoration(l) {
                             this._refreshStyle(l), this._dimensionsChanged && this._refreshXPosition(l);
                         }
                         _createElement(l) {
-                            var t;
+                            var e;
                             const s = this._coreBrowserService.mainDocument.createElement("div");
-                            s.classList.add("xterm-decoration"), s.classList.toggle("xterm-decoration-top-layer", ((t = l == null ? void 0 : l.options) == null ? void 0 : t.layer) === "top"), s.style.width = `${Math.round((l.options.width || 1) * this._renderService.dimensions.css.cell.width)}px`, s.style.height = (l.options.height || 1) * this._renderService.dimensions.css.cell.height + "px", s.style.top = (l.marker.line - this._bufferService.buffers.active.ydisp) * this._renderService.dimensions.css.cell.height + "px", s.style.lineHeight = `${this._renderService.dimensions.css.cell.height}px`;
+                            s.classList.add("xterm-decoration"), s.classList.toggle("xterm-decoration-top-layer", ((e = l == null ? void 0 : l.options) == null ? void 0 : e.layer) === "top"), s.style.width = `${Math.round((l.options.width || 1) * this._renderService.dimensions.css.cell.width)}px`, s.style.height = (l.options.height || 1) * this._renderService.dimensions.css.cell.height + "px", s.style.top = (l.marker.line - this._bufferService.buffers.active.ydisp) * this._renderService.dimensions.css.cell.height + "px", s.style.lineHeight = `${this._renderService.dimensions.css.cell.height}px`;
                             const r = l.options.x ?? 0;
                             return r && r > this._bufferService.cols && (s.style.display = "none"), this._refreshXPosition(l, s), s;
                         }
                         _refreshStyle(l) {
                             const s = l.marker.line - this._bufferService.buffers.active.ydisp;
                             if (s < 0 || s >= this._bufferService.rows)
                                 l.element && (l.element.style.display = "none", l.onRenderEmitter.fire(l.element));
@@ -3569,15 +3569,15 @@
                             (l.options.anchor || "left") === "right" ? s.style.right = r ? r * this._renderService.dimensions.css.cell.width + "px" : "": s.style.left = r ? r * this._renderService.dimensions.css.cell.width + "px" : "";
                         }
                         _removeDecoration(l) {
                             var s;
                             (s = this._decorationElements.get(l)) == null || s.remove(), this._decorationElements.delete(l), l.dispose();
                         }
                     };
-                    i.BufferDecorationRenderer = g = o([c(1, f.IBufferService), c(2, a.ICoreBrowserService), c(3, f.IDecorationService), c(4, a.IRenderService)], g);
+                    i.BufferDecorationRenderer = m = o([c(1, v.IBufferService), c(2, a.ICoreBrowserService), c(3, v.IDecorationService), c(4, a.IRenderService)], m);
                 },
                 5871: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.ColorZoneStore = void 0, i.ColorZoneStore = class {
                         constructor() {
                             this._zones = [], this._zonePool = [], this._zonePoolIndex = 0, this._linePadding = {
@@ -3623,36 +3623,36 @@
                         }
                         _addLineToZone(n, o) {
                             n.startBufferLine = Math.min(n.startBufferLine, o), n.endBufferLine = Math.max(n.endBufferLine, o);
                         }
                     };
                 },
                 5744: function(k, i, n) {
-                    var o = this && this.__decorate || function(e, h, v, u) {
-                            var p, _ = arguments.length,
-                                b = _ < 3 ? h : u === null ? u = Object.getOwnPropertyDescriptor(h, v) : u;
+                    var o = this && this.__decorate || function(t, h, g, u) {
+                            var S, _ = arguments.length,
+                                b = _ < 3 ? h : u === null ? u = Object.getOwnPropertyDescriptor(h, g) : u;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                b = Reflect.decorate(e, h, v, u);
+                                b = Reflect.decorate(t, h, g, u);
                             else
-                                for (var A = e.length - 1; A >= 0; A--)
-                                    (p = e[A]) && (b = (_ < 3 ? p(b) : _ > 3 ? p(h, v, b) : p(h, v)) || b);
-                            return _ > 3 && b && Object.defineProperty(h, v, b), b;
+                                for (var R = t.length - 1; R >= 0; R--)
+                                    (S = t[R]) && (b = (_ < 3 ? S(b) : _ > 3 ? S(h, g, b) : S(h, g)) || b);
+                            return _ > 3 && b && Object.defineProperty(h, g, b), b;
                         },
-                        c = this && this.__param || function(e, h) {
-                            return function(v, u) {
-                                h(v, u, e);
+                        c = this && this.__param || function(t, h) {
+                            return function(g, u) {
+                                h(g, u, t);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.OverviewRulerRenderer = void 0;
                     const a = n(5871),
                         d = n(4725),
-                        f = n(844),
-                        g = n(2585),
+                        v = n(844),
+                        m = n(2585),
                         l = {
                             full: 0,
                             left: 0,
                             center: 0,
                             right: 0
                         },
                         s = {
@@ -3663,27 +3663,27 @@
                         },
                         r = {
                             full: 0,
                             left: 0,
                             center: 0,
                             right: 0
                         };
-                    let t = i.OverviewRulerRenderer = class extends f.Disposable {
+                    let e = i.OverviewRulerRenderer = class extends v.Disposable {
                         get _width() {
                             return this._optionsService.options.overviewRulerWidth || 0;
                         }
-                        constructor(e, h, v, u, p, _, b) {
-                            var T;
-                            super(), this._viewportElement = e, this._screenElement = h, this._bufferService = v, this._decorationService = u, this._renderService = p, this._optionsService = _, this._coreBrowserService = b, this._colorZoneStore = new a.ColorZoneStore(), this._shouldUpdateDimensions = !0, this._shouldUpdateAnchor = !0, this._lastKnownBufferLength = 0, this._canvas = this._coreBrowserService.mainDocument.createElement("canvas"), this._canvas.classList.add("xterm-decoration-overview-ruler"), this._refreshCanvasDimensions(), (T = this._viewportElement.parentElement) == null || T.insertBefore(this._canvas, this._viewportElement);
-                            const A = this._canvas.getContext("2d");
-                            if (!A)
+                        constructor(t, h, g, u, S, _, b) {
+                            var B;
+                            super(), this._viewportElement = t, this._screenElement = h, this._bufferService = g, this._decorationService = u, this._renderService = S, this._optionsService = _, this._coreBrowserService = b, this._colorZoneStore = new a.ColorZoneStore(), this._shouldUpdateDimensions = !0, this._shouldUpdateAnchor = !0, this._lastKnownBufferLength = 0, this._canvas = this._coreBrowserService.mainDocument.createElement("canvas"), this._canvas.classList.add("xterm-decoration-overview-ruler"), this._refreshCanvasDimensions(), (B = this._viewportElement.parentElement) == null || B.insertBefore(this._canvas, this._viewportElement);
+                            const R = this._canvas.getContext("2d");
+                            if (!R)
                                 throw new Error("Ctx cannot be null");
-                            this._ctx = A, this._registerDecorationListeners(), this._registerBufferChangeListeners(), this._registerDimensionChangeListeners(), this.register((0, f.toDisposable)(() => {
-                                var x;
-                                (x = this._canvas) == null || x.remove();
+                            this._ctx = R, this._registerDecorationListeners(), this._registerBufferChangeListeners(), this._registerDimensionChangeListeners(), this.register((0, v.toDisposable)(() => {
+                                var T;
+                                (T = this._canvas) == null || T.remove();
                             }));
                         }
                         _registerDecorationListeners() {
                             this.register(this._decorationService.onDecorationRegistered(() => this._queueRefresh(void 0, !0))), this.register(this._decorationService.onDecorationRemoved(() => this._queueRefresh(void 0, !0)));
                         }
                         _registerBufferChangeListeners() {
                             this.register(this._renderService.onRenderedViewportChange(() => this._queueRefresh())), this.register(this._bufferService.buffers.onBufferActivate(() => {
@@ -3694,22 +3694,22 @@
                         }
                         _registerDimensionChangeListeners() {
                             this.register(this._renderService.onRender(() => {
                                 this._containerHeight && this._containerHeight === this._screenElement.clientHeight || (this._queueRefresh(!0), this._containerHeight = this._screenElement.clientHeight);
                             })), this.register(this._optionsService.onSpecificOptionChange("overviewRulerWidth", () => this._queueRefresh(!0))), this.register(this._coreBrowserService.onDprChange(() => this._queueRefresh(!0))), this._queueRefresh(!0);
                         }
                         _refreshDrawConstants() {
-                            const e = Math.floor(this._canvas.width / 3),
+                            const t = Math.floor(this._canvas.width / 3),
                                 h = Math.ceil(this._canvas.width / 3);
-                            s.full = this._canvas.width, s.left = e, s.center = h, s.right = e, this._refreshDrawHeightConstants(), r.full = 0, r.left = 0, r.center = s.left, r.right = s.left + s.center;
+                            s.full = this._canvas.width, s.left = t, s.center = h, s.right = t, this._refreshDrawHeightConstants(), r.full = 0, r.left = 0, r.center = s.left, r.right = s.left + s.center;
                         }
                         _refreshDrawHeightConstants() {
                             l.full = Math.round(2 * this._coreBrowserService.dpr);
-                            const e = this._canvas.height / this._bufferService.buffer.lines.length,
-                                h = Math.round(Math.max(Math.min(e, 12), 6) * this._coreBrowserService.dpr);
+                            const t = this._canvas.height / this._bufferService.buffer.lines.length,
+                                h = Math.round(Math.max(Math.min(t, 12), 6) * this._coreBrowserService.dpr);
                             l.left = h, l.center = h, l.right = h;
                         }
                         _refreshColorZonePadding() {
                             this._colorZoneStore.setPadding({
                                 full: Math.floor(this._bufferService.buffers.active.lines.length / (this._canvas.height - 1) * l.full),
                                 left: Math.floor(this._bufferService.buffers.active.lines.length / (this._canvas.height - 1) * l.left),
                                 center: Math.floor(this._bufferService.buffers.active.lines.length / (this._canvas.height - 1) * l.center),
@@ -3720,60 +3720,60 @@
                             this._canvas.style.width = `${this._width}px`, this._canvas.width = Math.round(this._width * this._coreBrowserService.dpr), this._canvas.style.height = `${this._screenElement.clientHeight}px`, this._canvas.height = Math.round(this._screenElement.clientHeight * this._coreBrowserService.dpr), this._refreshDrawConstants(), this._refreshColorZonePadding();
                         }
                         _refreshDecorations() {
                             this._shouldUpdateDimensions && this._refreshCanvasDimensions(), this._ctx.clearRect(0, 0, this._canvas.width, this._canvas.height), this._colorZoneStore.clear();
                             for (const h of this._decorationService.decorations)
                                 this._colorZoneStore.addDecoration(h);
                             this._ctx.lineWidth = 1;
-                            const e = this._colorZoneStore.zones;
-                            for (const h of e)
+                            const t = this._colorZoneStore.zones;
+                            for (const h of t)
                                 h.position !== "full" && this._renderColorZone(h);
-                            for (const h of e)
+                            for (const h of t)
                                 h.position === "full" && this._renderColorZone(h);
                             this._shouldUpdateDimensions = !1, this._shouldUpdateAnchor = !1;
                         }
-                        _renderColorZone(e) {
-                            this._ctx.fillStyle = e.color, this._ctx.fillRect(r[e.position || "full"], Math.round((this._canvas.height - 1) * (e.startBufferLine / this._bufferService.buffers.active.lines.length) - l[e.position || "full"] / 2), s[e.position || "full"], Math.round((this._canvas.height - 1) * ((e.endBufferLine - e.startBufferLine) / this._bufferService.buffers.active.lines.length) + l[e.position || "full"]));
+                        _renderColorZone(t) {
+                            this._ctx.fillStyle = t.color, this._ctx.fillRect(r[t.position || "full"], Math.round((this._canvas.height - 1) * (t.startBufferLine / this._bufferService.buffers.active.lines.length) - l[t.position || "full"] / 2), s[t.position || "full"], Math.round((this._canvas.height - 1) * ((t.endBufferLine - t.startBufferLine) / this._bufferService.buffers.active.lines.length) + l[t.position || "full"]));
                         }
-                        _queueRefresh(e, h) {
-                            this._shouldUpdateDimensions = e || this._shouldUpdateDimensions, this._shouldUpdateAnchor = h || this._shouldUpdateAnchor, this._animationFrame === void 0 && (this._animationFrame = this._coreBrowserService.window.requestAnimationFrame(() => {
+                        _queueRefresh(t, h) {
+                            this._shouldUpdateDimensions = t || this._shouldUpdateDimensions, this._shouldUpdateAnchor = h || this._shouldUpdateAnchor, this._animationFrame === void 0 && (this._animationFrame = this._coreBrowserService.window.requestAnimationFrame(() => {
                                 this._refreshDecorations(), this._animationFrame = void 0;
                             }));
                         }
                     };
-                    i.OverviewRulerRenderer = t = o([c(2, g.IBufferService), c(3, g.IDecorationService), c(4, d.IRenderService), c(5, g.IOptionsService), c(6, d.ICoreBrowserService)], t);
+                    i.OverviewRulerRenderer = e = o([c(2, m.IBufferService), c(3, m.IDecorationService), c(4, d.IRenderService), c(5, m.IOptionsService), c(6, d.ICoreBrowserService)], e);
                 },
                 2950: function(k, i, n) {
-                    var o = this && this.__decorate || function(l, s, r, t) {
-                            var e, h = arguments.length,
-                                v = h < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, r) : t;
+                    var o = this && this.__decorate || function(l, s, r, e) {
+                            var t, h = arguments.length,
+                                g = h < 3 ? s : e === null ? e = Object.getOwnPropertyDescriptor(s, r) : e;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                v = Reflect.decorate(l, s, r, t);
+                                g = Reflect.decorate(l, s, r, e);
                             else
                                 for (var u = l.length - 1; u >= 0; u--)
-                                    (e = l[u]) && (v = (h < 3 ? e(v) : h > 3 ? e(s, r, v) : e(s, r)) || v);
-                            return h > 3 && v && Object.defineProperty(s, r, v), v;
+                                    (t = l[u]) && (g = (h < 3 ? t(g) : h > 3 ? t(s, r, g) : t(s, r)) || g);
+                            return h > 3 && g && Object.defineProperty(s, r, g), g;
                         },
                         c = this && this.__param || function(l, s) {
-                            return function(r, t) {
-                                s(r, t, l);
+                            return function(r, e) {
+                                s(r, e, l);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CompositionHelper = void 0;
                     const a = n(4725),
                         d = n(2585),
-                        f = n(2584);
-                    let g = i.CompositionHelper = class {
+                        v = n(2584);
+                    let m = i.CompositionHelper = class {
                         get isComposing() {
                             return this._isComposing;
                         }
-                        constructor(l, s, r, t, e, h) {
-                            this._textarea = l, this._compositionView = s, this._bufferService = r, this._optionsService = t, this._coreService = e, this._renderService = h, this._isComposing = !1, this._isSendingComposition = !1, this._compositionPosition = {
+                        constructor(l, s, r, e, t, h) {
+                            this._textarea = l, this._compositionView = s, this._bufferService = r, this._optionsService = e, this._coreService = t, this._renderService = h, this._isComposing = !1, this._isSendingComposition = !1, this._compositionPosition = {
                                 start: 0,
                                 end: 0
                             }, this._dataAlreadySent = "";
                         }
                         compositionstart() {
                             this._isComposing = !0, this._compositionPosition.start = this._textarea.value.length, this._compositionView.textContent = "", this._dataAlreadySent = "", this._compositionView.classList.add("active");
                         }
@@ -3813,175 +3813,175 @@
                         }
                         _handleAnyTextareaChanges() {
                             const l = this._textarea.value;
                             setTimeout(() => {
                                 if (!this._isComposing) {
                                     const s = this._textarea.value,
                                         r = s.replace(l, "");
-                                    this._dataAlreadySent = r, s.length > l.length ? this._coreService.triggerDataEvent(r, !0) : s.length < l.length ? this._coreService.triggerDataEvent(`${f.C0.DEL}`, !0) : s.length === l.length && s !== l && this._coreService.triggerDataEvent(s, !0);
+                                    this._dataAlreadySent = r, s.length > l.length ? this._coreService.triggerDataEvent(r, !0) : s.length < l.length ? this._coreService.triggerDataEvent(`${v.C0.DEL}`, !0) : s.length === l.length && s !== l && this._coreService.triggerDataEvent(s, !0);
                                 }
                             }, 0);
                         }
                         updateCompositionElements(l) {
                             if (this._isComposing) {
                                 if (this._bufferService.buffer.isCursorInViewport) {
                                     const s = Math.min(this._bufferService.buffer.x, this._bufferService.cols - 1),
                                         r = this._renderService.dimensions.css.cell.height,
-                                        t = this._bufferService.buffer.y * this._renderService.dimensions.css.cell.height,
-                                        e = s * this._renderService.dimensions.css.cell.width;
-                                    this._compositionView.style.left = e + "px", this._compositionView.style.top = t + "px", this._compositionView.style.height = r + "px", this._compositionView.style.lineHeight = r + "px", this._compositionView.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._compositionView.style.fontSize = this._optionsService.rawOptions.fontSize + "px";
+                                        e = this._bufferService.buffer.y * this._renderService.dimensions.css.cell.height,
+                                        t = s * this._renderService.dimensions.css.cell.width;
+                                    this._compositionView.style.left = t + "px", this._compositionView.style.top = e + "px", this._compositionView.style.height = r + "px", this._compositionView.style.lineHeight = r + "px", this._compositionView.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._compositionView.style.fontSize = this._optionsService.rawOptions.fontSize + "px";
                                     const h = this._compositionView.getBoundingClientRect();
-                                    this._textarea.style.left = e + "px", this._textarea.style.top = t + "px", this._textarea.style.width = Math.max(h.width, 1) + "px", this._textarea.style.height = Math.max(h.height, 1) + "px", this._textarea.style.lineHeight = h.height + "px";
+                                    this._textarea.style.left = t + "px", this._textarea.style.top = e + "px", this._textarea.style.width = Math.max(h.width, 1) + "px", this._textarea.style.height = Math.max(h.height, 1) + "px", this._textarea.style.lineHeight = h.height + "px";
                                 }
                                 l || setTimeout(() => this.updateCompositionElements(!0), 0);
                             }
                         }
                     };
-                    i.CompositionHelper = g = o([c(2, d.IBufferService), c(3, d.IOptionsService), c(4, d.ICoreService), c(5, a.IRenderService)], g);
+                    i.CompositionHelper = m = o([c(2, d.IBufferService), c(3, d.IOptionsService), c(4, d.ICoreService), c(5, a.IRenderService)], m);
                 },
                 9806: (k, i) => {
                     function n(o, c, a) {
                         const d = a.getBoundingClientRect(),
-                            f = o.getComputedStyle(a),
-                            g = parseInt(f.getPropertyValue("padding-left")),
-                            l = parseInt(f.getPropertyValue("padding-top"));
-                        return [c.clientX - d.left - g, c.clientY - d.top - l];
+                            v = o.getComputedStyle(a),
+                            m = parseInt(v.getPropertyValue("padding-left")),
+                            l = parseInt(v.getPropertyValue("padding-top"));
+                        return [c.clientX - d.left - m, c.clientY - d.top - l];
                     }
                     Object.defineProperty(i, "__esModule", {
                         value: !0
-                    }), i.getCoords = i.getCoordsRelativeToElement = void 0, i.getCoordsRelativeToElement = n, i.getCoords = function(o, c, a, d, f, g, l, s, r) {
-                        if (!g)
+                    }), i.getCoords = i.getCoordsRelativeToElement = void 0, i.getCoordsRelativeToElement = n, i.getCoords = function(o, c, a, d, v, m, l, s, r) {
+                        if (!m)
                             return;
-                        const t = n(o, c, a);
-                        return t ? (t[0] = Math.ceil((t[0] + (r ? l / 2 : 0)) / l), t[1] = Math.ceil(t[1] / s), t[0] = Math.min(Math.max(t[0], 1), d + (r ? 1 : 0)), t[1] = Math.min(Math.max(t[1], 1), f), t) : void 0;
+                        const e = n(o, c, a);
+                        return e ? (e[0] = Math.ceil((e[0] + (r ? l / 2 : 0)) / l), e[1] = Math.ceil(e[1] / s), e[0] = Math.min(Math.max(e[0], 1), d + (r ? 1 : 0)), e[1] = Math.min(Math.max(e[1], 1), v), e) : void 0;
                     };
                 },
                 9504: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.moveToCellSequence = void 0;
                     const o = n(2584);
 
-                    function c(s, r, t, e) {
-                        const h = s - a(s, t),
-                            v = r - a(r, t),
-                            u = Math.abs(h - v) - function(p, _, b) {
-                                let A = 0;
-                                const T = p - a(p, b),
-                                    x = _ - a(_, b);
-                                for (let L = 0; L < Math.abs(T - x); L++) {
-                                    const H = d(p, _) === "A" ? -1 : 1,
-                                        W = b.buffer.lines.get(T + H * L);
-                                    W != null && W.isWrapped && A++;
-                                }
-                                return A;
-                            }(s, r, t);
-                        return l(u, g(d(s, r), e));
+                    function c(s, r, e, t) {
+                        const h = s - a(s, e),
+                            g = r - a(r, e),
+                            u = Math.abs(h - g) - function(S, _, b) {
+                                let R = 0;
+                                const B = S - a(S, b),
+                                    T = _ - a(_, b);
+                                for (let L = 0; L < Math.abs(B - T); L++) {
+                                    const H = d(S, _) === "A" ? -1 : 1,
+                                        W = b.buffer.lines.get(B + H * L);
+                                    W != null && W.isWrapped && R++;
+                                }
+                                return R;
+                            }(s, r, e);
+                        return l(u, m(d(s, r), t));
                     }
 
                     function a(s, r) {
-                        let t = 0,
-                            e = r.buffer.lines.get(s),
-                            h = e == null ? void 0 : e.isWrapped;
+                        let e = 0,
+                            t = r.buffer.lines.get(s),
+                            h = t == null ? void 0 : t.isWrapped;
                         for (; h && s >= 0 && s < r.rows;)
-                            t++, e = r.buffer.lines.get(--s), h = e == null ? void 0 : e.isWrapped;
-                        return t;
+                            e++, t = r.buffer.lines.get(--s), h = t == null ? void 0 : t.isWrapped;
+                        return e;
                     }
 
                     function d(s, r) {
                         return s > r ? "A" : "B";
                     }
 
-                    function f(s, r, t, e, h, v) {
+                    function v(s, r, e, t, h, g) {
                         let u = s,
-                            p = r,
+                            S = r,
                             _ = "";
-                        for (; u !== t || p !== e;)
-                            u += h ? 1 : -1, h && u > v.cols - 1 ? (_ += v.buffer.translateBufferLineToString(p, !1, s, u), u = 0, s = 0, p++) : !h && u < 0 && (_ += v.buffer.translateBufferLineToString(p, !1, 0, s + 1), u = v.cols - 1, s = u, p--);
-                        return _ + v.buffer.translateBufferLineToString(p, !1, s, u);
+                        for (; u !== e || S !== t;)
+                            u += h ? 1 : -1, h && u > g.cols - 1 ? (_ += g.buffer.translateBufferLineToString(S, !1, s, u), u = 0, s = 0, S++) : !h && u < 0 && (_ += g.buffer.translateBufferLineToString(S, !1, 0, s + 1), u = g.cols - 1, s = u, S--);
+                        return _ + g.buffer.translateBufferLineToString(S, !1, s, u);
                     }
 
-                    function g(s, r) {
-                        const t = r ? "O" : "[";
-                        return o.C0.ESC + t + s;
+                    function m(s, r) {
+                        const e = r ? "O" : "[";
+                        return o.C0.ESC + e + s;
                     }
 
                     function l(s, r) {
                         s = Math.floor(s);
-                        let t = "";
-                        for (let e = 0; e < s; e++)
-                            t += r;
-                        return t;
-                    }
-                    i.moveToCellSequence = function(s, r, t, e) {
-                        const h = t.buffer.x,
-                            v = t.buffer.y;
-                        if (!t.buffer.hasScrollback)
-                            return function(_, b, A, T, x, L) {
-                                return c(b, T, x, L).length === 0 ? "" : l(f(_, b, _, b - a(b, x), !1, x).length, g("D", L));
-                            }(h, v, 0, r, t, e) + c(v, r, t, e) + function(_, b, A, T, x, L) {
+                        let e = "";
+                        for (let t = 0; t < s; t++)
+                            e += r;
+                        return e;
+                    }
+                    i.moveToCellSequence = function(s, r, e, t) {
+                        const h = e.buffer.x,
+                            g = e.buffer.y;
+                        if (!e.buffer.hasScrollback)
+                            return function(_, b, R, B, T, L) {
+                                return c(b, B, T, L).length === 0 ? "" : l(v(_, b, _, b - a(b, T), !1, T).length, m("D", L));
+                            }(h, g, 0, r, e, t) + c(g, r, e, t) + function(_, b, R, B, T, L) {
                                 let H;
-                                H = c(b, T, x, L).length > 0 ? T - a(T, x) : b;
-                                const W = T,
-                                    U = function(K, j, C, D, B, O) {
+                                H = c(b, B, T, L).length > 0 ? B - a(B, T) : b;
+                                const W = B,
+                                    j = function(V, z, C, x, A, O) {
                                         let I;
-                                        return I = c(C, D, B, O).length > 0 ? D - a(D, B) : j, K < C && I <= D || K >= C && I < D ? "C" : "D";
-                                    }(_, b, A, T, x, L);
-                                return l(f(_, H, A, W, U === "C", x).length, g(U, L));
-                            }(h, v, s, r, t, e);
+                                        return I = c(C, x, A, O).length > 0 ? x - a(x, A) : z, V < C && I <= x || V >= C && I < x ? "C" : "D";
+                                    }(_, b, R, B, T, L);
+                                return l(v(_, H, R, W, j === "C", T).length, m(j, L));
+                            }(h, g, s, r, e, t);
                         let u;
-                        if (v === r)
-                            return u = h > s ? "D" : "C", l(Math.abs(h - s), g(u, e));
-                        u = v > r ? "D" : "C";
-                        const p = Math.abs(v - r);
+                        if (g === r)
+                            return u = h > s ? "D" : "C", l(Math.abs(h - s), m(u, t));
+                        u = g > r ? "D" : "C";
+                        const S = Math.abs(g - r);
                         return l(function(_, b) {
                             return b.cols - _;
-                        }(v > r ? s : h, t) + (p - 1) * t.cols + 1 + ((v > r ? h : s) - 1), g(u, e));
+                        }(g > r ? s : h, e) + (S - 1) * e.cols + 1 + ((g > r ? h : s) - 1), m(u, t));
                     };
                 },
                 1296: function(k, i, n) {
-                    var o = this && this.__decorate || function(L, H, W, U) {
-                            var K, j = arguments.length,
-                                C = j < 3 ? H : U === null ? U = Object.getOwnPropertyDescriptor(H, W) : U;
+                    var o = this && this.__decorate || function(L, H, W, j) {
+                            var V, z = arguments.length,
+                                C = z < 3 ? H : j === null ? j = Object.getOwnPropertyDescriptor(H, W) : j;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                C = Reflect.decorate(L, H, W, U);
+                                C = Reflect.decorate(L, H, W, j);
                             else
-                                for (var D = L.length - 1; D >= 0; D--)
-                                    (K = L[D]) && (C = (j < 3 ? K(C) : j > 3 ? K(H, W, C) : K(H, W)) || C);
-                            return j > 3 && C && Object.defineProperty(H, W, C), C;
+                                for (var x = L.length - 1; x >= 0; x--)
+                                    (V = L[x]) && (C = (z < 3 ? V(C) : z > 3 ? V(H, W, C) : V(H, W)) || C);
+                            return z > 3 && C && Object.defineProperty(H, W, C), C;
                         },
                         c = this && this.__param || function(L, H) {
-                            return function(W, U) {
-                                H(W, U, L);
+                            return function(W, j) {
+                                H(W, j, L);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.DomRenderer = void 0;
                     const a = n(3787),
                         d = n(2550),
-                        f = n(2223),
-                        g = n(6171),
+                        v = n(2223),
+                        m = n(6171),
                         l = n(6052),
                         s = n(4725),
                         r = n(8055),
-                        t = n(8460),
-                        e = n(844),
+                        e = n(8460),
+                        t = n(844),
                         h = n(2585),
-                        v = "xterm-dom-renderer-owner-",
+                        g = "xterm-dom-renderer-owner-",
                         u = "xterm-rows",
-                        p = "xterm-fg-",
+                        S = "xterm-fg-",
                         _ = "xterm-bg-",
                         b = "xterm-focus",
-                        A = "xterm-selection";
-                    let T = 1,
-                        x = i.DomRenderer = class extends e.Disposable {
-                            constructor(L, H, W, U, K, j, C, D, B, O, I, z, G) {
-                                super(), this._terminal = L, this._document = H, this._element = W, this._screenElement = U, this._viewportElement = K, this._helperContainer = j, this._linkifier2 = C, this._charSizeService = B, this._optionsService = O, this._bufferService = I, this._coreBrowserService = z, this._themeService = G, this._terminalClass = T++, this._rowElements = [], this._selectionRenderModel = (0, l.createSelectionRenderModel)(), this.onRequestRedraw = this.register(new t.EventEmitter()).event, this._rowContainer = this._document.createElement("div"), this._rowContainer.classList.add(u), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = this._document.createElement("div"), this._selectionContainer.classList.add(A), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, g.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange(() => this._handleOptionsChanged())), this.register(this._themeService.onChangeColors((X) => this._injectCss(X))), this._injectCss(this._themeService.colors), this._rowFactory = D.createInstance(a.DomRendererRowFactory, document), this._element.classList.add(v + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline((X) => this._handleLinkHover(X))), this.register(this._linkifier2.onHideLinkUnderline((X) => this._handleLinkLeave(X))), this.register((0, e.toDisposable)(() => {
-                                    this._element.classList.remove(v + this._terminalClass), this._rowContainer.remove(), this._selectionContainer.remove(), this._widthCache.dispose(), this._themeStyleElement.remove(), this._dimensionsStyleElement.remove();
+                        R = "xterm-selection";
+                    let B = 1,
+                        T = i.DomRenderer = class extends t.Disposable {
+                            constructor(L, H, W, j, V, z, C, x, A, O, I, q, X) {
+                                super(), this._terminal = L, this._document = H, this._element = W, this._screenElement = j, this._viewportElement = V, this._helperContainer = z, this._linkifier2 = C, this._charSizeService = A, this._optionsService = O, this._bufferService = I, this._coreBrowserService = q, this._themeService = X, this._terminalClass = B++, this._rowElements = [], this._selectionRenderModel = (0, l.createSelectionRenderModel)(), this.onRequestRedraw = this.register(new e.EventEmitter()).event, this._rowContainer = this._document.createElement("div"), this._rowContainer.classList.add(u), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = this._document.createElement("div"), this._selectionContainer.classList.add(R), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, m.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange(() => this._handleOptionsChanged())), this.register(this._themeService.onChangeColors((J) => this._injectCss(J))), this._injectCss(this._themeService.colors), this._rowFactory = x.createInstance(a.DomRendererRowFactory, document), this._element.classList.add(g + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline((J) => this._handleLinkHover(J))), this.register(this._linkifier2.onHideLinkUnderline((J) => this._handleLinkLeave(J))), this.register((0, t.toDisposable)(() => {
+                                    this._element.classList.remove(g + this._terminalClass), this._rowContainer.remove(), this._selectionContainer.remove(), this._widthCache.dispose(), this._themeStyleElement.remove(), this._dimensionsStyleElement.remove();
                                 })), this._widthCache = new d.WidthCache(this._document, this._helperContainer), this._widthCache.setFont(this._optionsService.rawOptions.fontFamily, this._optionsService.rawOptions.fontSize, this._optionsService.rawOptions.fontWeight, this._optionsService.rawOptions.fontWeightBold), this._setDefaultSpacing();
                             }
                             _updateDimensions() {
                                 const L = this._coreBrowserService.dpr;
                                 this.dimensions.device.char.width = this._charSizeService.width * L, this.dimensions.device.char.height = Math.ceil(this._charSizeService.height * L), this.dimensions.device.cell.width = this.dimensions.device.char.width + Math.round(this._optionsService.rawOptions.letterSpacing), this.dimensions.device.cell.height = Math.floor(this.dimensions.device.char.height * this._optionsService.rawOptions.lineHeight), this.dimensions.device.char.left = 0, this.dimensions.device.char.top = 0, this.dimensions.device.canvas.width = this.dimensions.device.cell.width * this._bufferService.cols, this.dimensions.device.canvas.height = this.dimensions.device.cell.height * this._bufferService.rows, this.dimensions.css.canvas.width = Math.round(this.dimensions.device.canvas.width / L), this.dimensions.css.canvas.height = Math.round(this.dimensions.device.canvas.height / L), this.dimensions.css.cell.width = this.dimensions.css.canvas.width / this._bufferService.cols, this.dimensions.css.cell.height = this.dimensions.css.canvas.height / this._bufferService.rows;
                                 for (const W of this._rowElements)
                                     W.style.width = `${this.dimensions.css.canvas.width}px`, W.style.height = `${this.dimensions.css.cell.height}px`, W.style.lineHeight = `${this.dimensions.css.cell.height}px`, W.style.overflow = "hidden";
@@ -3990,32 +3990,32 @@
                                 this._dimensionsStyleElement.textContent = H, this._selectionContainer.style.height = this._viewportElement.style.height, this._screenElement.style.width = `${this.dimensions.css.canvas.width}px`, this._screenElement.style.height = `${this.dimensions.css.canvas.height}px`;
                             }
                             _injectCss(L) {
                                 this._themeStyleElement || (this._themeStyleElement = this._document.createElement("style"), this._screenElement.appendChild(this._themeStyleElement));
                                 let H = `${this._terminalSelector} .${u} { color: ${L.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px; font-kerning: none; white-space: pre}`;
                                 H += `${this._terminalSelector} .${u} .xterm-dim { color: ${r.color.multiplyOpacity(L.foreground, 0.5).css};}`, H += `${this._terminalSelector} span:not(.xterm-bold) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.xterm-bold { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.xterm-italic { font-style: italic;}`;
                                 const W = `blink_underline_${this._terminalClass}`,
-                                    U = `blink_bar_${this._terminalClass}`,
-                                    K = `blink_block_${this._terminalClass}`;
-                                H += `@keyframes ${W} { 50% {  border-bottom-style: hidden; }}`, H += `@keyframes ${U} { 50% {  box-shadow: none; }}`, H += `@keyframes ${K} { 0% {  background-color: ${L.cursor.css};  color: ${L.cursorAccent.css}; } 50% {  background-color: inherit;  color: ${L.cursor.css}; }}`, H += `${this._terminalSelector} .${u}.${b} .xterm-cursor.xterm-cursor-blink.xterm-cursor-underline { animation: ${W} 1s step-end infinite;}${this._terminalSelector} .${u}.${b} .xterm-cursor.xterm-cursor-blink.xterm-cursor-bar { animation: ${U} 1s step-end infinite;}${this._terminalSelector} .${u}.${b} .xterm-cursor.xterm-cursor-blink.xterm-cursor-block { animation: ${K} 1s step-end infinite;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-block { background-color: ${L.cursor.css}; color: ${L.cursorAccent.css};}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-block:not(.xterm-cursor-blink) { background-color: ${L.cursor.css} !important; color: ${L.cursorAccent.css} !important;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-outline { outline: 1px solid ${L.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-bar { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${L.cursor.css} inset;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-underline { border-bottom: 1px ${L.cursor.css}; border-bottom-style: solid; height: calc(100% - 1px);}`, H += `${this._terminalSelector} .${A} { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .${A} div { position: absolute; background-color: ${L.selectionBackgroundOpaque.css};}${this._terminalSelector} .${A} div { position: absolute; background-color: ${L.selectionInactiveBackgroundOpaque.css};}`;
-                                for (const [j, C] of L.ansi.entries())
-                                    H += `${this._terminalSelector} .${p}${j} { color: ${C.css}; }${this._terminalSelector} .${p}${j}.xterm-dim { color: ${r.color.multiplyOpacity(C, 0.5).css}; }${this._terminalSelector} .${_}${j} { background-color: ${C.css}; }`;
-                                H += `${this._terminalSelector} .${p}${f.INVERTED_DEFAULT_COLOR} { color: ${r.color.opaque(L.background).css}; }${this._terminalSelector} .${p}${f.INVERTED_DEFAULT_COLOR}.xterm-dim { color: ${r.color.multiplyOpacity(r.color.opaque(L.background), 0.5).css}; }${this._terminalSelector} .${_}${f.INVERTED_DEFAULT_COLOR} { background-color: ${L.foreground.css}; }`, this._themeStyleElement.textContent = H;
+                                    j = `blink_bar_${this._terminalClass}`,
+                                    V = `blink_block_${this._terminalClass}`;
+                                H += `@keyframes ${W} { 50% {  border-bottom-style: hidden; }}`, H += `@keyframes ${j} { 50% {  box-shadow: none; }}`, H += `@keyframes ${V} { 0% {  background-color: ${L.cursor.css};  color: ${L.cursorAccent.css}; } 50% {  background-color: inherit;  color: ${L.cursor.css}; }}`, H += `${this._terminalSelector} .${u}.${b} .xterm-cursor.xterm-cursor-blink.xterm-cursor-underline { animation: ${W} 1s step-end infinite;}${this._terminalSelector} .${u}.${b} .xterm-cursor.xterm-cursor-blink.xterm-cursor-bar { animation: ${j} 1s step-end infinite;}${this._terminalSelector} .${u}.${b} .xterm-cursor.xterm-cursor-blink.xterm-cursor-block { animation: ${V} 1s step-end infinite;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-block { background-color: ${L.cursor.css}; color: ${L.cursorAccent.css};}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-block:not(.xterm-cursor-blink) { background-color: ${L.cursor.css} !important; color: ${L.cursorAccent.css} !important;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-outline { outline: 1px solid ${L.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-bar { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${L.cursor.css} inset;}${this._terminalSelector} .${u} .xterm-cursor.xterm-cursor-underline { border-bottom: 1px ${L.cursor.css}; border-bottom-style: solid; height: calc(100% - 1px);}`, H += `${this._terminalSelector} .${R} { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .${R} div { position: absolute; background-color: ${L.selectionBackgroundOpaque.css};}${this._terminalSelector} .${R} div { position: absolute; background-color: ${L.selectionInactiveBackgroundOpaque.css};}`;
+                                for (const [z, C] of L.ansi.entries())
+                                    H += `${this._terminalSelector} .${S}${z} { color: ${C.css}; }${this._terminalSelector} .${S}${z}.xterm-dim { color: ${r.color.multiplyOpacity(C, 0.5).css}; }${this._terminalSelector} .${_}${z} { background-color: ${C.css}; }`;
+                                H += `${this._terminalSelector} .${S}${v.INVERTED_DEFAULT_COLOR} { color: ${r.color.opaque(L.background).css}; }${this._terminalSelector} .${S}${v.INVERTED_DEFAULT_COLOR}.xterm-dim { color: ${r.color.multiplyOpacity(r.color.opaque(L.background), 0.5).css}; }${this._terminalSelector} .${_}${v.INVERTED_DEFAULT_COLOR} { background-color: ${L.foreground.css}; }`, this._themeStyleElement.textContent = H;
                             }
                             _setDefaultSpacing() {
                                 const L = this.dimensions.css.cell.width - this._widthCache.get("W", !1, !1);
                                 this._rowContainer.style.letterSpacing = `${L}px`, this._rowFactory.defaultSpacing = L;
                             }
                             handleDevicePixelRatioChange() {
                                 this._updateDimensions(), this._widthCache.clear(), this._setDefaultSpacing();
                             }
                             _refreshRowElements(L, H) {
                                 for (let W = this._rowElements.length; W <= H; W++) {
-                                    const U = this._document.createElement("div");
-                                    this._rowContainer.appendChild(U), this._rowElements.push(U);
+                                    const j = this._document.createElement("div");
+                                    this._rowContainer.appendChild(j), this._rowElements.push(j);
                                 }
                                 for (; this._rowElements.length > H;)
                                     this._rowContainer.removeChild(this._rowElements.pop());
                             }
                             handleResize(L, H) {
                                 this._refreshRowElements(L, H), this._updateDimensions(), this.handleSelectionChanged(this._selectionRenderModel.selectionStart, this._selectionRenderModel.selectionEnd, this._selectionRenderModel.columnSelectMode);
                             }
@@ -4028,290 +4028,290 @@
                             handleFocus() {
                                 this._rowContainer.classList.add(b), this.renderRows(this._bufferService.buffer.y, this._bufferService.buffer.y);
                             }
                             handleSelectionChanged(L, H, W) {
                                 if (this._selectionContainer.replaceChildren(), this._rowFactory.handleSelectionChanged(L, H, W), this.renderRows(0, this._bufferService.rows - 1), !L || !H)
                                     return;
                                 this._selectionRenderModel.update(this._terminal, L, H, W);
-                                const U = this._selectionRenderModel.viewportStartRow,
-                                    K = this._selectionRenderModel.viewportEndRow,
-                                    j = this._selectionRenderModel.viewportCappedStartRow,
+                                const j = this._selectionRenderModel.viewportStartRow,
+                                    V = this._selectionRenderModel.viewportEndRow,
+                                    z = this._selectionRenderModel.viewportCappedStartRow,
                                     C = this._selectionRenderModel.viewportCappedEndRow;
-                                if (j >= this._bufferService.rows || C < 0)
+                                if (z >= this._bufferService.rows || C < 0)
                                     return;
-                                const D = this._document.createDocumentFragment();
+                                const x = this._document.createDocumentFragment();
                                 if (W) {
-                                    const B = L[0] > H[0];
-                                    D.appendChild(this._createSelectionElement(j, B ? H[0] : L[0], B ? L[0] : H[0], C - j + 1));
+                                    const A = L[0] > H[0];
+                                    x.appendChild(this._createSelectionElement(z, A ? H[0] : L[0], A ? L[0] : H[0], C - z + 1));
                                 } else {
-                                    const B = U === j ? L[0] : 0,
-                                        O = j === K ? H[0] : this._bufferService.cols;
-                                    D.appendChild(this._createSelectionElement(j, B, O));
-                                    const I = C - j - 1;
-                                    if (D.appendChild(this._createSelectionElement(j + 1, 0, this._bufferService.cols, I)), j !== C) {
-                                        const z = K === C ? H[0] : this._bufferService.cols;
-                                        D.appendChild(this._createSelectionElement(C, 0, z));
+                                    const A = j === z ? L[0] : 0,
+                                        O = z === V ? H[0] : this._bufferService.cols;
+                                    x.appendChild(this._createSelectionElement(z, A, O));
+                                    const I = C - z - 1;
+                                    if (x.appendChild(this._createSelectionElement(z + 1, 0, this._bufferService.cols, I)), z !== C) {
+                                        const q = V === C ? H[0] : this._bufferService.cols;
+                                        x.appendChild(this._createSelectionElement(C, 0, q));
                                     }
                                 }
-                                this._selectionContainer.appendChild(D);
+                                this._selectionContainer.appendChild(x);
                             }
-                            _createSelectionElement(L, H, W, U = 1) {
-                                const K = this._document.createElement("div"),
-                                    j = H * this.dimensions.css.cell.width;
+                            _createSelectionElement(L, H, W, j = 1) {
+                                const V = this._document.createElement("div"),
+                                    z = H * this.dimensions.css.cell.width;
                                 let C = this.dimensions.css.cell.width * (W - H);
-                                return j + C > this.dimensions.css.canvas.width && (C = this.dimensions.css.canvas.width - j), K.style.height = U * this.dimensions.css.cell.height + "px", K.style.top = L * this.dimensions.css.cell.height + "px", K.style.left = `${j}px`, K.style.width = `${C}px`, K;
+                                return z + C > this.dimensions.css.canvas.width && (C = this.dimensions.css.canvas.width - z), V.style.height = j * this.dimensions.css.cell.height + "px", V.style.top = L * this.dimensions.css.cell.height + "px", V.style.left = `${z}px`, V.style.width = `${C}px`, V;
                             }
                             handleCursorMove() {}
                             _handleOptionsChanged() {
                                 this._updateDimensions(), this._injectCss(this._themeService.colors), this._widthCache.setFont(this._optionsService.rawOptions.fontFamily, this._optionsService.rawOptions.fontSize, this._optionsService.rawOptions.fontWeight, this._optionsService.rawOptions.fontWeightBold), this._setDefaultSpacing();
                             }
                             clear() {
                                 for (const L of this._rowElements)
                                     L.replaceChildren();
                             }
                             renderRows(L, H) {
                                 const W = this._bufferService.buffer,
-                                    U = W.ybase + W.y,
-                                    K = Math.min(W.x, this._bufferService.cols - 1),
-                                    j = this._optionsService.rawOptions.cursorBlink,
+                                    j = W.ybase + W.y,
+                                    V = Math.min(W.x, this._bufferService.cols - 1),
+                                    z = this._optionsService.rawOptions.cursorBlink,
                                     C = this._optionsService.rawOptions.cursorStyle,
-                                    D = this._optionsService.rawOptions.cursorInactiveStyle;
-                                for (let B = L; B <= H; B++) {
-                                    const O = B + W.ydisp,
-                                        I = this._rowElements[B],
-                                        z = W.lines.get(O);
-                                    if (!I || !z)
+                                    x = this._optionsService.rawOptions.cursorInactiveStyle;
+                                for (let A = L; A <= H; A++) {
+                                    const O = A + W.ydisp,
+                                        I = this._rowElements[A],
+                                        q = W.lines.get(O);
+                                    if (!I || !q)
                                         break;
-                                    I.replaceChildren(...this._rowFactory.createRow(z, O, O === U, C, D, K, j, this.dimensions.css.cell.width, this._widthCache, -1, -1));
+                                    I.replaceChildren(...this._rowFactory.createRow(q, O, O === j, C, x, V, z, this.dimensions.css.cell.width, this._widthCache, -1, -1));
                                 }
                             }
                             get _terminalSelector() {
-                                return `.${v}${this._terminalClass}`;
+                                return `.${g}${this._terminalClass}`;
                             }
                             _handleLinkHover(L) {
                                 this._setCellUnderline(L.x1, L.x2, L.y1, L.y2, L.cols, !0);
                             }
                             _handleLinkLeave(L) {
                                 this._setCellUnderline(L.x1, L.x2, L.y1, L.y2, L.cols, !1);
                             }
-                            _setCellUnderline(L, H, W, U, K, j) {
-                                W < 0 && (L = 0), U < 0 && (H = 0);
+                            _setCellUnderline(L, H, W, j, V, z) {
+                                W < 0 && (L = 0), j < 0 && (H = 0);
                                 const C = this._bufferService.rows - 1;
-                                W = Math.max(Math.min(W, C), 0), U = Math.max(Math.min(U, C), 0), K = Math.min(K, this._bufferService.cols);
-                                const D = this._bufferService.buffer,
-                                    B = D.ybase + D.y,
-                                    O = Math.min(D.x, K - 1),
+                                W = Math.max(Math.min(W, C), 0), j = Math.max(Math.min(j, C), 0), V = Math.min(V, this._bufferService.cols);
+                                const x = this._bufferService.buffer,
+                                    A = x.ybase + x.y,
+                                    O = Math.min(x.x, V - 1),
                                     I = this._optionsService.rawOptions.cursorBlink,
-                                    z = this._optionsService.rawOptions.cursorStyle,
-                                    G = this._optionsService.rawOptions.cursorInactiveStyle;
-                                for (let X = W; X <= U; ++X) {
-                                    const P = X + D.ydisp,
-                                        w = this._rowElements[X],
-                                        N = D.lines.get(P);
-                                    if (!w || !N)
+                                    q = this._optionsService.rawOptions.cursorStyle,
+                                    X = this._optionsService.rawOptions.cursorInactiveStyle;
+                                for (let J = W; J <= j; ++J) {
+                                    const P = J + x.ydisp,
+                                        w = this._rowElements[J],
+                                        U = x.lines.get(P);
+                                    if (!w || !U)
                                         break;
-                                    w.replaceChildren(...this._rowFactory.createRow(N, P, P === B, z, G, O, I, this.dimensions.css.cell.width, this._widthCache, j ? X === W ? L : 0 : -1, j ? (X === U ? H : K) - 1 : -1));
+                                    w.replaceChildren(...this._rowFactory.createRow(U, P, P === A, q, X, O, I, this.dimensions.css.cell.width, this._widthCache, z ? J === W ? L : 0 : -1, z ? (J === j ? H : V) - 1 : -1));
                                 }
                             }
                         };
-                    i.DomRenderer = x = o([c(7, h.IInstantiationService), c(8, s.ICharSizeService), c(9, h.IOptionsService), c(10, h.IBufferService), c(11, s.ICoreBrowserService), c(12, s.IThemeService)], x);
+                    i.DomRenderer = T = o([c(7, h.IInstantiationService), c(8, s.ICharSizeService), c(9, h.IOptionsService), c(10, h.IBufferService), c(11, s.ICoreBrowserService), c(12, s.IThemeService)], T);
                 },
                 3787: function(k, i, n) {
-                    var o = this && this.__decorate || function(u, p, _, b) {
-                            var A, T = arguments.length,
-                                x = T < 3 ? p : b === null ? b = Object.getOwnPropertyDescriptor(p, _) : b;
+                    var o = this && this.__decorate || function(u, S, _, b) {
+                            var R, B = arguments.length,
+                                T = B < 3 ? S : b === null ? b = Object.getOwnPropertyDescriptor(S, _) : b;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                x = Reflect.decorate(u, p, _, b);
+                                T = Reflect.decorate(u, S, _, b);
                             else
                                 for (var L = u.length - 1; L >= 0; L--)
-                                    (A = u[L]) && (x = (T < 3 ? A(x) : T > 3 ? A(p, _, x) : A(p, _)) || x);
-                            return T > 3 && x && Object.defineProperty(p, _, x), x;
+                                    (R = u[L]) && (T = (B < 3 ? R(T) : B > 3 ? R(S, _, T) : R(S, _)) || T);
+                            return B > 3 && T && Object.defineProperty(S, _, T), T;
                         },
-                        c = this && this.__param || function(u, p) {
+                        c = this && this.__param || function(u, S) {
                             return function(_, b) {
-                                p(_, b, u);
+                                S(_, b, u);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.DomRendererRowFactory = void 0;
                     const a = n(2223),
                         d = n(643),
-                        f = n(511),
-                        g = n(2585),
+                        v = n(511),
+                        m = n(2585),
                         l = n(8055),
                         s = n(4725),
                         r = n(4269),
-                        t = n(6171),
-                        e = n(3734);
+                        e = n(6171),
+                        t = n(3734);
                     let h = i.DomRendererRowFactory = class {
-                        constructor(u, p, _, b, A, T, x) {
-                            this._document = u, this._characterJoinerService = p, this._optionsService = _, this._coreBrowserService = b, this._coreService = A, this._decorationService = T, this._themeService = x, this._workCell = new f.CellData(), this._columnSelectMode = !1, this.defaultSpacing = 0;
+                        constructor(u, S, _, b, R, B, T) {
+                            this._document = u, this._characterJoinerService = S, this._optionsService = _, this._coreBrowserService = b, this._coreService = R, this._decorationService = B, this._themeService = T, this._workCell = new v.CellData(), this._columnSelectMode = !1, this.defaultSpacing = 0;
                         }
-                        handleSelectionChanged(u, p, _) {
-                            this._selectionStart = u, this._selectionEnd = p, this._columnSelectMode = _;
+                        handleSelectionChanged(u, S, _) {
+                            this._selectionStart = u, this._selectionEnd = S, this._columnSelectMode = _;
                         }
-                        createRow(u, p, _, b, A, T, x, L, H, W, U) {
-                            const K = [],
-                                j = this._characterJoinerService.getJoinedCharacters(p),
+                        createRow(u, S, _, b, R, B, T, L, H, W, j) {
+                            const V = [],
+                                z = this._characterJoinerService.getJoinedCharacters(S),
                                 C = this._themeService.colors;
-                            let D, B = u.getNoBgTrimmedLength();
-                            _ && B < T + 1 && (B = T + 1);
+                            let x, A = u.getNoBgTrimmedLength();
+                            _ && A < B + 1 && (A = B + 1);
                             let O = 0,
                                 I = "",
-                                z = 0,
-                                G = 0,
+                                q = 0,
                                 X = 0,
+                                J = 0,
                                 P = !1,
                                 w = 0,
-                                N = !1,
+                                U = !1,
                                 F = 0;
-                            const V = [],
-                                q = W !== -1 && U !== -1;
-                            for (let Z = 0; Z < B; Z++) {
-                                u.loadCell(Z, this._workCell);
-                                let ie = this._workCell.getWidth();
-                                if (ie === 0)
+                            const G = [],
+                                K = W !== -1 && j !== -1;
+                            for (let ee = 0; ee < A; ee++) {
+                                u.loadCell(ee, this._workCell);
+                                let se = this._workCell.getWidth();
+                                if (se === 0)
                                     continue;
-                                let se = !1,
-                                    re = Z,
-                                    J = this._workCell;
-                                if (j.length > 0 && Z === j[0][0]) {
-                                    se = !0;
-                                    const ee = j.shift();
-                                    J = new r.JoinedCellData(this._workCell, u.translateToString(!0, ee[0], ee[1]), ee[1] - ee[0]), re = ee[1] - 1, ie = J.getWidth();
-                                }
-                                const Ae = this._isCellInSelection(Z, p),
-                                    qe = _ && Z === T,
-                                    Ke = q && Z >= W && Z <= U;
+                                let ie = !1,
+                                    oe = ee,
+                                    Z = this._workCell;
+                                if (z.length > 0 && ee === z[0][0]) {
+                                    ie = !0;
+                                    const re = z.shift();
+                                    Z = new r.JoinedCellData(this._workCell, u.translateToString(!0, re[0], re[1]), re[1] - re[0]), oe = re[1] - 1, se = Z.getWidth();
+                                }
+                                const N = this._isCellInSelection(ee, S),
+                                    we = _ && ee === B,
+                                    Ke = K && ee >= W && ee <= j;
                                 let Ve = !1;
-                                this._decorationService.forEachDecorationAtCell(Z, p, void 0, (ee) => {
+                                this._decorationService.forEachDecorationAtCell(ee, S, void 0, (re) => {
                                     Ve = !0;
                                 });
-                                let Pe = J.getChars() || d.WHITESPACE_CELL_CHAR;
-                                if (Pe === " " && (J.isUnderline() || J.isOverline()) && (Pe = " "), F = ie * L - H.get(Pe, J.isBold(), J.isItalic()), D) {
-                                    if (O && (Ae && N || !Ae && !N && J.bg === z) && (Ae && N && C.selectionForeground || J.fg === G) && J.extended.ext === X && Ke === P && F === w && !qe && !se && !Ve) {
-                                        J.isInvisible() ? I += d.WHITESPACE_CELL_CHAR : I += Pe, O++;
+                                let Ie = Z.getChars() || d.WHITESPACE_CELL_CHAR;
+                                if (Ie === " " && (Z.isUnderline() || Z.isOverline()) && (Ie = " "), F = se * L - H.get(Ie, Z.isBold(), Z.isItalic()), x) {
+                                    if (O && (N && U || !N && !U && Z.bg === q) && (N && U && C.selectionForeground || Z.fg === X) && Z.extended.ext === J && Ke === P && F === w && !we && !ie && !Ve) {
+                                        Z.isInvisible() ? I += d.WHITESPACE_CELL_CHAR : I += Ie, O++;
                                         continue;
                                     }
-                                    O && (D.textContent = I), D = this._document.createElement("span"), O = 0, I = "";
+                                    O && (x.textContent = I), x = this._document.createElement("span"), O = 0, I = "";
                                 } else
-                                    D = this._document.createElement("span");
-                                if (z = J.bg, G = J.fg, X = J.extended.ext, P = Ke, w = F, N = Ae, se && T >= Z && T <= re && (T = Z), !this._coreService.isCursorHidden && qe && this._coreService.isCursorInitialized) {
-                                    if (V.push("xterm-cursor"), this._coreBrowserService.isFocused)
-                                        x && V.push("xterm-cursor-blink"), V.push(b === "bar" ? "xterm-cursor-bar" : b === "underline" ? "xterm-cursor-underline" : "xterm-cursor-block");
-                                    else if (A)
-                                        switch (A) {
+                                    x = this._document.createElement("span");
+                                if (q = Z.bg, X = Z.fg, J = Z.extended.ext, P = Ke, w = F, U = N, ie && B >= ee && B <= oe && (B = ee), !this._coreService.isCursorHidden && we && this._coreService.isCursorInitialized) {
+                                    if (G.push("xterm-cursor"), this._coreBrowserService.isFocused)
+                                        T && G.push("xterm-cursor-blink"), G.push(b === "bar" ? "xterm-cursor-bar" : b === "underline" ? "xterm-cursor-underline" : "xterm-cursor-block");
+                                    else if (R)
+                                        switch (R) {
                                             case "outline":
-                                                V.push("xterm-cursor-outline");
+                                                G.push("xterm-cursor-outline");
                                                 break;
                                             case "block":
-                                                V.push("xterm-cursor-block");
+                                                G.push("xterm-cursor-block");
                                                 break;
                                             case "bar":
-                                                V.push("xterm-cursor-bar");
+                                                G.push("xterm-cursor-bar");
                                                 break;
                                             case "underline":
-                                                V.push("xterm-cursor-underline");
+                                                G.push("xterm-cursor-underline");
                                         }
                                 }
-                                if (J.isBold() && V.push("xterm-bold"), J.isItalic() && V.push("xterm-italic"), J.isDim() && V.push("xterm-dim"), I = J.isInvisible() ? d.WHITESPACE_CELL_CHAR : J.getChars() || d.WHITESPACE_CELL_CHAR, J.isUnderline() && (V.push(`xterm-underline-${J.extended.underlineStyle}`), I === " " && (I = " "), !J.isUnderlineColorDefault()))
-                                    if (J.isUnderlineColorRGB())
-                                        D.style.textDecorationColor = `rgb(${e.AttributeData.toColorRGB(J.getUnderlineColor()).join(",")})`;
+                                if (Z.isBold() && G.push("xterm-bold"), Z.isItalic() && G.push("xterm-italic"), Z.isDim() && G.push("xterm-dim"), I = Z.isInvisible() ? d.WHITESPACE_CELL_CHAR : Z.getChars() || d.WHITESPACE_CELL_CHAR, Z.isUnderline() && (G.push(`xterm-underline-${Z.extended.underlineStyle}`), I === " " && (I = " "), !Z.isUnderlineColorDefault()))
+                                    if (Z.isUnderlineColorRGB())
+                                        x.style.textDecorationColor = `rgb(${t.AttributeData.toColorRGB(Z.getUnderlineColor()).join(",")})`;
                                     else {
-                                        let ee = J.getUnderlineColor();
-                                        this._optionsService.rawOptions.drawBoldTextInBrightColors && J.isBold() && ee < 8 && (ee += 8), D.style.textDecorationColor = C.ansi[ee].css;
+                                        let re = Z.getUnderlineColor();
+                                        this._optionsService.rawOptions.drawBoldTextInBrightColors && Z.isBold() && re < 8 && (re += 8), x.style.textDecorationColor = C.ansi[re].css;
                                     }
-                                J.isOverline() && (V.push("xterm-overline"), I === " " && (I = " ")), J.isStrikethrough() && V.push("xterm-strikethrough"), Ke && (D.style.textDecoration = "underline");
-                                let oe = J.getFgColor(),
-                                    Be = J.getFgColorMode(),
-                                    de = J.getBgColor(),
-                                    Te = J.getBgColorMode();
-                                const Ge = !!J.isInverse();
+                                Z.isOverline() && (G.push("xterm-overline"), I === " " && (I = " ")), Z.isStrikethrough() && G.push("xterm-strikethrough"), Ke && (x.style.textDecoration = "underline");
+                                let he = Z.getFgColor(),
+                                    Be = Z.getFgColorMode(),
+                                    ue = Z.getBgColor(),
+                                    Me = Z.getBgColorMode();
+                                const Ge = !!Z.isInverse();
                                 if (Ge) {
-                                    const ee = oe;
-                                    oe = de, de = ee;
+                                    const re = he;
+                                    he = ue, ue = re;
                                     const qt = Be;
-                                    Be = Te, Te = qt;
+                                    Be = Me, Me = qt;
                                 }
-                                let pe, Ie, me, Me = !1;
-                                switch (this._decorationService.forEachDecorationAtCell(Z, p, void 0, (ee) => {
-                                        ee.options.layer !== "top" && Me || (ee.backgroundColorRGB && (Te = 50331648, de = ee.backgroundColorRGB.rgba >> 8 & 16777215, pe = ee.backgroundColorRGB), ee.foregroundColorRGB && (Be = 50331648, oe = ee.foregroundColorRGB.rgba >> 8 & 16777215, Ie = ee.foregroundColorRGB), Me = ee.options.layer === "top");
-                                    }), !Me && Ae && (pe = this._coreBrowserService.isFocused ? C.selectionBackgroundOpaque : C.selectionInactiveBackgroundOpaque, de = pe.rgba >> 8 & 16777215, Te = 50331648, Me = !0, C.selectionForeground && (Be = 50331648, oe = C.selectionForeground.rgba >> 8 & 16777215, Ie = C.selectionForeground)), Me && V.push("xterm-decoration-top"), Te) {
+                                let pe, He, Se, Te = !1;
+                                switch (this._decorationService.forEachDecorationAtCell(ee, S, void 0, (re) => {
+                                        re.options.layer !== "top" && Te || (re.backgroundColorRGB && (Me = 50331648, ue = re.backgroundColorRGB.rgba >> 8 & 16777215, pe = re.backgroundColorRGB), re.foregroundColorRGB && (Be = 50331648, he = re.foregroundColorRGB.rgba >> 8 & 16777215, He = re.foregroundColorRGB), Te = re.options.layer === "top");
+                                    }), !Te && N && (pe = this._coreBrowserService.isFocused ? C.selectionBackgroundOpaque : C.selectionInactiveBackgroundOpaque, ue = pe.rgba >> 8 & 16777215, Me = 50331648, Te = !0, C.selectionForeground && (Be = 50331648, he = C.selectionForeground.rgba >> 8 & 16777215, He = C.selectionForeground)), Te && G.push("xterm-decoration-top"), Me) {
                                     case 16777216:
                                     case 33554432:
-                                        me = C.ansi[de], V.push(`xterm-bg-${de}`);
+                                        Se = C.ansi[ue], G.push(`xterm-bg-${ue}`);
                                         break;
                                     case 50331648:
-                                        me = l.channels.toColor(de >> 16, de >> 8 & 255, 255 & de), this._addStyle(D, `background-color:#${v((de >>> 0).toString(16), "0", 6)}`);
+                                        Se = l.channels.toColor(ue >> 16, ue >> 8 & 255, 255 & ue), this._addStyle(x, `background-color:#${g((ue >>> 0).toString(16), "0", 6)}`);
                                         break;
                                     default:
-                                        Ge ? (me = C.foreground, V.push(`xterm-bg-${a.INVERTED_DEFAULT_COLOR}`)) : me = C.background;
+                                        Ge ? (Se = C.foreground, G.push(`xterm-bg-${a.INVERTED_DEFAULT_COLOR}`)) : Se = C.background;
                                 }
-                                switch (pe || J.isDim() && (pe = l.color.multiplyOpacity(me, 0.5)), Be) {
+                                switch (pe || Z.isDim() && (pe = l.color.multiplyOpacity(Se, 0.5)), Be) {
                                     case 16777216:
                                     case 33554432:
-                                        J.isBold() && oe < 8 && this._optionsService.rawOptions.drawBoldTextInBrightColors && (oe += 8), this._applyMinimumContrast(D, me, C.ansi[oe], J, pe, void 0) || V.push(`xterm-fg-${oe}`);
+                                        Z.isBold() && he < 8 && this._optionsService.rawOptions.drawBoldTextInBrightColors && (he += 8), this._applyMinimumContrast(x, Se, C.ansi[he], Z, pe, void 0) || G.push(`xterm-fg-${he}`);
                                         break;
                                     case 50331648:
-                                        const ee = l.channels.toColor(oe >> 16 & 255, oe >> 8 & 255, 255 & oe);
-                                        this._applyMinimumContrast(D, me, ee, J, pe, Ie) || this._addStyle(D, `color:#${v(oe.toString(16), "0", 6)}`);
+                                        const re = l.channels.toColor(he >> 16 & 255, he >> 8 & 255, 255 & he);
+                                        this._applyMinimumContrast(x, Se, re, Z, pe, He) || this._addStyle(x, `color:#${g(he.toString(16), "0", 6)}`);
                                         break;
                                     default:
-                                        this._applyMinimumContrast(D, me, C.foreground, J, pe, Ie) || Ge && V.push(`xterm-fg-${a.INVERTED_DEFAULT_COLOR}`);
+                                        this._applyMinimumContrast(x, Se, C.foreground, Z, pe, He) || Ge && G.push(`xterm-fg-${a.INVERTED_DEFAULT_COLOR}`);
                                 }
-                                V.length && (D.className = V.join(" "), V.length = 0), qe || se || Ve ? D.textContent = I : O++, F !== this.defaultSpacing && (D.style.letterSpacing = `${F}px`), K.push(D), Z = re;
+                                G.length && (x.className = G.join(" "), G.length = 0), we || ie || Ve ? x.textContent = I : O++, F !== this.defaultSpacing && (x.style.letterSpacing = `${F}px`), V.push(x), ee = oe;
                             }
-                            return D && O && (D.textContent = I), K;
+                            return x && O && (x.textContent = I), V;
                         }
-                        _applyMinimumContrast(u, p, _, b, A, T) {
-                            if (this._optionsService.rawOptions.minimumContrastRatio === 1 || (0, t.treatGlyphAsBackgroundColor)(b.getCode()))
+                        _applyMinimumContrast(u, S, _, b, R, B) {
+                            if (this._optionsService.rawOptions.minimumContrastRatio === 1 || (0, e.treatGlyphAsBackgroundColor)(b.getCode()))
                                 return !1;
-                            const x = this._getContrastCache(b);
+                            const T = this._getContrastCache(b);
                             let L;
-                            if (A || T || (L = x.getColor(p.rgba, _.rgba)), L === void 0) {
+                            if (R || B || (L = T.getColor(S.rgba, _.rgba)), L === void 0) {
                                 const H = this._optionsService.rawOptions.minimumContrastRatio / (b.isDim() ? 2 : 1);
-                                L = l.color.ensureContrastRatio(A || p, T || _, H), x.setColor((A || p).rgba, (T || _).rgba, L ?? null);
+                                L = l.color.ensureContrastRatio(R || S, B || _, H), T.setColor((R || S).rgba, (B || _).rgba, L ?? null);
                             }
                             return !!L && (this._addStyle(u, `color:${L.css}`), !0);
                         }
                         _getContrastCache(u) {
                             return u.isDim() ? this._themeService.colors.halfContrastCache : this._themeService.colors.contrastCache;
                         }
-                        _addStyle(u, p) {
-                            u.setAttribute("style", `${u.getAttribute("style") || ""}${p};`);
+                        _addStyle(u, S) {
+                            u.setAttribute("style", `${u.getAttribute("style") || ""}${S};`);
                         }
-                        _isCellInSelection(u, p) {
+                        _isCellInSelection(u, S) {
                             const _ = this._selectionStart,
                                 b = this._selectionEnd;
-                            return !(!_ || !b) && (this._columnSelectMode ? _[0] <= b[0] ? u >= _[0] && p >= _[1] && u < b[0] && p <= b[1] : u < _[0] && p >= _[1] && u >= b[0] && p <= b[1] : p > _[1] && p < b[1] || _[1] === b[1] && p === _[1] && u >= _[0] && u < b[0] || _[1] < b[1] && p === b[1] && u < b[0] || _[1] < b[1] && p === _[1] && u >= _[0]);
+                            return !(!_ || !b) && (this._columnSelectMode ? _[0] <= b[0] ? u >= _[0] && S >= _[1] && u < b[0] && S <= b[1] : u < _[0] && S >= _[1] && u >= b[0] && S <= b[1] : S > _[1] && S < b[1] || _[1] === b[1] && S === _[1] && u >= _[0] && u < b[0] || _[1] < b[1] && S === b[1] && u < b[0] || _[1] < b[1] && S === _[1] && u >= _[0]);
                         }
                     };
 
-                    function v(u, p, _) {
+                    function g(u, S, _) {
                         for (; u.length < _;)
-                            u = p + u;
+                            u = S + u;
                         return u;
                     }
-                    i.DomRendererRowFactory = h = o([c(1, s.ICharacterJoinerService), c(2, g.IOptionsService), c(3, s.ICoreBrowserService), c(4, g.ICoreService), c(5, g.IDecorationService), c(6, s.IThemeService)], h);
+                    i.DomRendererRowFactory = h = o([c(1, s.ICharacterJoinerService), c(2, m.IOptionsService), c(3, s.ICoreBrowserService), c(4, m.ICoreService), c(5, m.IDecorationService), c(6, s.IThemeService)], h);
                 },
                 2550: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.WidthCache = void 0, i.WidthCache = class {
                         constructor(n, o) {
                             this._flat = new Float32Array(256), this._font = "", this._fontSize = 0, this._weight = "normal", this._weightBold = "bold", this._measureElements = [], this._container = n.createElement("div"), this._container.classList.add("xterm-width-cache-measure-container"), this._container.setAttribute("aria-hidden", "true"), this._container.style.whiteSpace = "pre", this._container.style.fontKerning = "none";
                             const c = n.createElement("span");
                             c.classList.add("xterm-char-measure-element");
                             const a = n.createElement("span");
                             a.classList.add("xterm-char-measure-element"), a.style.fontWeight = "bold";
                             const d = n.createElement("span");
                             d.classList.add("xterm-char-measure-element"), d.style.fontStyle = "italic";
-                            const f = n.createElement("span");
-                            f.classList.add("xterm-char-measure-element"), f.style.fontWeight = "bold", f.style.fontStyle = "italic", this._measureElements = [c, a, d, f], this._container.appendChild(c), this._container.appendChild(a), this._container.appendChild(d), this._container.appendChild(f), o.appendChild(this._container), this.clear();
+                            const v = n.createElement("span");
+                            v.classList.add("xterm-char-measure-element"), v.style.fontWeight = "bold", v.style.fontStyle = "italic", this._measureElements = [c, a, d, v], this._container.appendChild(c), this._container.appendChild(a), this._container.appendChild(d), this._container.appendChild(v), o.appendChild(this._container), this.clear();
                         }
                         dispose() {
                             this._container.remove(), this._measureElements.length = 0, this._holey = void 0;
                         }
                         clear() {
                             this._flat.fill(-9999), this._holey = /* @__PURE__ */ new Map();
                         }
@@ -4319,25 +4319,25 @@
                             n === this._font && o === this._fontSize && c === this._weight && a === this._weightBold || (this._font = n, this._fontSize = o, this._weight = c, this._weightBold = a, this._container.style.fontFamily = this._font, this._container.style.fontSize = `${this._fontSize}px`, this._measureElements[0].style.fontWeight = `${c}`, this._measureElements[1].style.fontWeight = `${a}`, this._measureElements[2].style.fontWeight = `${c}`, this._measureElements[3].style.fontWeight = `${a}`, this.clear());
                         }
                         get(n, o, c) {
                             let a = 0;
                             if (!o && !c && n.length === 1 && (a = n.charCodeAt(0)) < 256) {
                                 if (this._flat[a] !== -9999)
                                     return this._flat[a];
-                                const g = this._measure(n, 0);
-                                return g > 0 && (this._flat[a] = g), g;
+                                const m = this._measure(n, 0);
+                                return m > 0 && (this._flat[a] = m), m;
                             }
                             let d = n;
                             o && (d += "B"), c && (d += "I");
-                            let f = this._holey.get(d);
-                            if (f === void 0) {
-                                let g = 0;
-                                o && (g |= 1), c && (g |= 2), f = this._measure(n, g), f > 0 && this._holey.set(d, f);
+                            let v = this._holey.get(d);
+                            if (v === void 0) {
+                                let m = 0;
+                                o && (m |= 1), c && (m |= 2), v = this._measure(n, m), v > 0 && this._holey.set(d, v);
                             }
-                            return f;
+                            return v;
                         }
                         _measure(n, o) {
                             const c = this._measureElements[o];
                             return c.textContent = n.repeat(32), c.offsetWidth / 32;
                         }
                     };
                 },
@@ -4360,17 +4360,17 @@
                         value: !0
                     }), i.computeNextVariantOffset = i.createRenderDimensions = i.treatGlyphAsBackgroundColor = i.allowRescaling = i.isEmoji = i.isRestrictedPowerlineGlyph = i.isPowerlineGlyph = i.throwIfFalsy = void 0, i.throwIfFalsy = function(c) {
                         if (!c)
                             throw new Error("value must not be falsy");
                         return c;
                     }, i.isPowerlineGlyph = n, i.isRestrictedPowerlineGlyph = function(c) {
                         return 57520 <= c && c <= 57527;
-                    }, i.isEmoji = o, i.allowRescaling = function(c, a, d, f) {
-                        return a === 1 && d > Math.ceil(1.5 * f) && c !== void 0 && c > 255 && !o(c) && !n(c) && ! function(g) {
-                            return 57344 <= g && g <= 63743;
+                    }, i.isEmoji = o, i.allowRescaling = function(c, a, d, v) {
+                        return a === 1 && d > Math.ceil(1.5 * v) && c !== void 0 && c > 255 && !o(c) && !n(c) && ! function(m) {
+                            return 57344 <= m && m <= 63743;
                         }(c);
                     }, i.treatGlyphAsBackgroundColor = function(c) {
                         return n(c) || function(a) {
                             return 9472 <= a && a <= 9631;
                         }(c);
                     }, i.createRenderDimensions = function() {
                         return {
@@ -4412,23 +4412,23 @@
                     class n {
                         constructor() {
                             this.clear();
                         }
                         clear() {
                             this.hasSelection = !1, this.columnSelectMode = !1, this.viewportStartRow = 0, this.viewportEndRow = 0, this.viewportCappedStartRow = 0, this.viewportCappedEndRow = 0, this.startCol = 0, this.endCol = 0, this.selectionStart = void 0, this.selectionEnd = void 0;
                         }
-                        update(c, a, d, f = !1) {
+                        update(c, a, d, v = !1) {
                             if (this.selectionStart = a, this.selectionEnd = d, !a || !d || a[0] === d[0] && a[1] === d[1])
                                 return void this.clear();
-                            const g = c.buffers.active.ydisp,
-                                l = a[1] - g,
-                                s = d[1] - g,
+                            const m = c.buffers.active.ydisp,
+                                l = a[1] - m,
+                                s = d[1] - m,
                                 r = Math.max(l, 0),
-                                t = Math.min(s, c.rows - 1);
-                            r >= c.rows || t < 0 ? this.clear() : (this.hasSelection = !0, this.columnSelectMode = f, this.viewportStartRow = l, this.viewportEndRow = s, this.viewportCappedStartRow = r, this.viewportCappedEndRow = t, this.startCol = a[0], this.endCol = d[0]);
+                                e = Math.min(s, c.rows - 1);
+                            r >= c.rows || e < 0 ? this.clear() : (this.hasSelection = !0, this.columnSelectMode = v, this.viewportStartRow = l, this.viewportEndRow = s, this.viewportCappedStartRow = r, this.viewportCappedEndRow = e, this.startCol = a[0], this.endCol = d[0]);
                         }
                         isCellSelected(c, a, d) {
                             return !!this.hasSelection && (d -= c.buffer.active.viewportY, this.columnSelectMode ? this.startCol <= this.endCol ? a >= this.startCol && d >= this.viewportCappedStartRow && a < this.endCol && d <= this.viewportCappedEndRow : a < this.startCol && d >= this.viewportCappedStartRow && a >= this.endCol && d <= this.viewportCappedEndRow : d > this.viewportStartRow && d < this.viewportEndRow || this.viewportStartRow === this.viewportEndRow && d === this.viewportStartRow && a >= this.startCol && a < this.endCol || this.viewportStartRow < this.viewportEndRow && d === this.viewportEndRow && a < this.endCol || this.viewportStartRow < this.viewportEndRow && d === this.viewportStartRow && a >= this.startCol);
                         }
                     }
                     i.createSelectionRenderModel = function() {
                         return new n();
@@ -4469,255 +4469,255 @@
                         }
                         handleTrim(n) {
                             return this.selectionStart && (this.selectionStart[1] -= n), this.selectionEnd && (this.selectionEnd[1] -= n), this.selectionEnd && this.selectionEnd[1] < 0 ? (this.clearSelection(), !0) : (this.selectionStart && this.selectionStart[1] < 0 && (this.selectionStart[1] = 0), !1);
                         }
                     };
                 },
                 428: function(k, i, n) {
-                    var o = this && this.__decorate || function(t, e, h, v) {
-                            var u, p = arguments.length,
-                                _ = p < 3 ? e : v === null ? v = Object.getOwnPropertyDescriptor(e, h) : v;
+                    var o = this && this.__decorate || function(e, t, h, g) {
+                            var u, S = arguments.length,
+                                _ = S < 3 ? t : g === null ? g = Object.getOwnPropertyDescriptor(t, h) : g;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                _ = Reflect.decorate(t, e, h, v);
+                                _ = Reflect.decorate(e, t, h, g);
                             else
-                                for (var b = t.length - 1; b >= 0; b--)
-                                    (u = t[b]) && (_ = (p < 3 ? u(_) : p > 3 ? u(e, h, _) : u(e, h)) || _);
-                            return p > 3 && _ && Object.defineProperty(e, h, _), _;
+                                for (var b = e.length - 1; b >= 0; b--)
+                                    (u = e[b]) && (_ = (S < 3 ? u(_) : S > 3 ? u(t, h, _) : u(t, h)) || _);
+                            return S > 3 && _ && Object.defineProperty(t, h, _), _;
                         },
-                        c = this && this.__param || function(t, e) {
-                            return function(h, v) {
-                                e(h, v, t);
+                        c = this && this.__param || function(e, t) {
+                            return function(h, g) {
+                                t(h, g, e);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CharSizeService = void 0;
                     const a = n(2585),
                         d = n(8460),
-                        f = n(844);
-                    let g = i.CharSizeService = class extends f.Disposable {
+                        v = n(844);
+                    let m = i.CharSizeService = class extends v.Disposable {
                         get hasValidSize() {
                             return this.width > 0 && this.height > 0;
                         }
-                        constructor(t, e, h) {
+                        constructor(e, t, h) {
                             super(), this._optionsService = h, this.width = 0, this.height = 0, this._onCharSizeChange = this.register(new d.EventEmitter()), this.onCharSizeChange = this._onCharSizeChange.event;
                             try {
                                 this._measureStrategy = this.register(new r(this._optionsService));
                             } catch {
-                                this._measureStrategy = this.register(new s(t, e, this._optionsService));
+                                this._measureStrategy = this.register(new s(e, t, this._optionsService));
                             }
                             this.register(this._optionsService.onMultipleOptionChange(["fontFamily", "fontSize"], () => this.measure()));
                         }
                         measure() {
-                            const t = this._measureStrategy.measure();
-                            t.width === this.width && t.height === this.height || (this.width = t.width, this.height = t.height, this._onCharSizeChange.fire());
+                            const e = this._measureStrategy.measure();
+                            e.width === this.width && e.height === this.height || (this.width = e.width, this.height = e.height, this._onCharSizeChange.fire());
                         }
                     };
-                    i.CharSizeService = g = o([c(2, a.IOptionsService)], g);
-                    class l extends f.Disposable {
+                    i.CharSizeService = m = o([c(2, a.IOptionsService)], m);
+                    class l extends v.Disposable {
                         constructor() {
                             super(...arguments), this._result = {
                                 width: 0,
                                 height: 0
                             };
                         }
-                        _validateAndSet(e, h) {
-                            e !== void 0 && e > 0 && h !== void 0 && h > 0 && (this._result.width = e, this._result.height = h);
+                        _validateAndSet(t, h) {
+                            t !== void 0 && t > 0 && h !== void 0 && h > 0 && (this._result.width = t, this._result.height = h);
                         }
                     }
                     class s extends l {
-                        constructor(e, h, v) {
-                            super(), this._document = e, this._parentElement = h, this._optionsService = v, this._measureElement = this._document.createElement("span"), this._measureElement.classList.add("xterm-char-measure-element"), this._measureElement.textContent = "W".repeat(32), this._measureElement.setAttribute("aria-hidden", "true"), this._measureElement.style.whiteSpace = "pre", this._measureElement.style.fontKerning = "none", this._parentElement.appendChild(this._measureElement);
+                        constructor(t, h, g) {
+                            super(), this._document = t, this._parentElement = h, this._optionsService = g, this._measureElement = this._document.createElement("span"), this._measureElement.classList.add("xterm-char-measure-element"), this._measureElement.textContent = "W".repeat(32), this._measureElement.setAttribute("aria-hidden", "true"), this._measureElement.style.whiteSpace = "pre", this._measureElement.style.fontKerning = "none", this._parentElement.appendChild(this._measureElement);
                         }
                         measure() {
                             return this._measureElement.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._measureElement.style.fontSize = `${this._optionsService.rawOptions.fontSize}px`, this._validateAndSet(Number(this._measureElement.offsetWidth) / 32, Number(this._measureElement.offsetHeight)), this._result;
                         }
                     }
                     class r extends l {
-                        constructor(e) {
-                            super(), this._optionsService = e, this._canvas = new OffscreenCanvas(100, 100), this._ctx = this._canvas.getContext("2d");
+                        constructor(t) {
+                            super(), this._optionsService = t, this._canvas = new OffscreenCanvas(100, 100), this._ctx = this._canvas.getContext("2d");
                             const h = this._ctx.measureText("W");
                             if (!("width" in h && "fontBoundingBoxAscent" in h && "fontBoundingBoxDescent" in h))
                                 throw new Error("Required font metrics not supported");
                         }
                         measure() {
                             this._ctx.font = `${this._optionsService.rawOptions.fontSize}px ${this._optionsService.rawOptions.fontFamily}`;
-                            const e = this._ctx.measureText("W");
-                            return this._validateAndSet(e.width, e.fontBoundingBoxAscent + e.fontBoundingBoxDescent), this._result;
+                            const t = this._ctx.measureText("W");
+                            return this._validateAndSet(t.width, t.fontBoundingBoxAscent + t.fontBoundingBoxDescent), this._result;
                         }
                     }
                 },
                 4269: function(k, i, n) {
-                    var o = this && this.__decorate || function(r, t, e, h) {
-                            var v, u = arguments.length,
-                                p = u < 3 ? t : h === null ? h = Object.getOwnPropertyDescriptor(t, e) : h;
+                    var o = this && this.__decorate || function(r, e, t, h) {
+                            var g, u = arguments.length,
+                                S = u < 3 ? e : h === null ? h = Object.getOwnPropertyDescriptor(e, t) : h;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                p = Reflect.decorate(r, t, e, h);
+                                S = Reflect.decorate(r, e, t, h);
                             else
                                 for (var _ = r.length - 1; _ >= 0; _--)
-                                    (v = r[_]) && (p = (u < 3 ? v(p) : u > 3 ? v(t, e, p) : v(t, e)) || p);
-                            return u > 3 && p && Object.defineProperty(t, e, p), p;
+                                    (g = r[_]) && (S = (u < 3 ? g(S) : u > 3 ? g(e, t, S) : g(e, t)) || S);
+                            return u > 3 && S && Object.defineProperty(e, t, S), S;
                         },
-                        c = this && this.__param || function(r, t) {
-                            return function(e, h) {
-                                t(e, h, r);
+                        c = this && this.__param || function(r, e) {
+                            return function(t, h) {
+                                e(t, h, r);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CharacterJoinerService = i.JoinedCellData = void 0;
                     const a = n(3734),
                         d = n(643),
-                        f = n(511),
-                        g = n(2585);
+                        v = n(511),
+                        m = n(2585);
                     class l extends a.AttributeData {
-                        constructor(t, e, h) {
-                            super(), this.content = 0, this.combinedData = "", this.fg = t.fg, this.bg = t.bg, this.combinedData = e, this._width = h;
+                        constructor(e, t, h) {
+                            super(), this.content = 0, this.combinedData = "", this.fg = e.fg, this.bg = e.bg, this.combinedData = t, this._width = h;
                         }
                         isCombined() {
                             return 2097152;
                         }
                         getWidth() {
                             return this._width;
                         }
                         getChars() {
                             return this.combinedData;
                         }
                         getCode() {
                             return 2097151;
                         }
-                        setFromCharData(t) {
+                        setFromCharData(e) {
                             throw new Error("not implemented");
                         }
                         getAsCharData() {
                             return [this.fg, this.getChars(), this.getWidth(), this.getCode()];
                         }
                     }
                     i.JoinedCellData = l;
                     let s = i.CharacterJoinerService = class jt {
-                        constructor(t) {
-                            this._bufferService = t, this._characterJoiners = [], this._nextCharacterJoinerId = 0, this._workCell = new f.CellData();
+                        constructor(e) {
+                            this._bufferService = e, this._characterJoiners = [], this._nextCharacterJoinerId = 0, this._workCell = new v.CellData();
                         }
-                        register(t) {
-                            const e = {
+                        register(e) {
+                            const t = {
                                 id: this._nextCharacterJoinerId++,
-                                handler: t
+                                handler: e
                             };
-                            return this._characterJoiners.push(e), e.id;
+                            return this._characterJoiners.push(t), t.id;
                         }
-                        deregister(t) {
-                            for (let e = 0; e < this._characterJoiners.length; e++)
-                                if (this._characterJoiners[e].id === t)
-                                    return this._characterJoiners.splice(e, 1), !0;
+                        deregister(e) {
+                            for (let t = 0; t < this._characterJoiners.length; t++)
+                                if (this._characterJoiners[t].id === e)
+                                    return this._characterJoiners.splice(t, 1), !0;
                             return !1;
                         }
-                        getJoinedCharacters(t) {
+                        getJoinedCharacters(e) {
                             if (this._characterJoiners.length === 0)
                                 return [];
-                            const e = this._bufferService.buffer.lines.get(t);
-                            if (!e || e.length === 0)
+                            const t = this._bufferService.buffer.lines.get(e);
+                            if (!t || t.length === 0)
                                 return [];
                             const h = [],
-                                v = e.translateToString(!0);
+                                g = t.translateToString(!0);
                             let u = 0,
-                                p = 0,
+                                S = 0,
                                 _ = 0,
-                                b = e.getFg(0),
-                                A = e.getBg(0);
-                            for (let T = 0; T < e.getTrimmedLength(); T++)
-                                if (e.loadCell(T, this._workCell), this._workCell.getWidth() !== 0) {
-                                    if (this._workCell.fg !== b || this._workCell.bg !== A) {
-                                        if (T - u > 1) {
-                                            const x = this._getJoinedRanges(v, _, p, e, u);
-                                            for (let L = 0; L < x.length; L++)
-                                                h.push(x[L]);
+                                b = t.getFg(0),
+                                R = t.getBg(0);
+                            for (let B = 0; B < t.getTrimmedLength(); B++)
+                                if (t.loadCell(B, this._workCell), this._workCell.getWidth() !== 0) {
+                                    if (this._workCell.fg !== b || this._workCell.bg !== R) {
+                                        if (B - u > 1) {
+                                            const T = this._getJoinedRanges(g, _, S, t, u);
+                                            for (let L = 0; L < T.length; L++)
+                                                h.push(T[L]);
                                         }
-                                        u = T, _ = p, b = this._workCell.fg, A = this._workCell.bg;
+                                        u = B, _ = S, b = this._workCell.fg, R = this._workCell.bg;
                                     }
-                                    p += this._workCell.getChars().length || d.WHITESPACE_CELL_CHAR.length;
+                                    S += this._workCell.getChars().length || d.WHITESPACE_CELL_CHAR.length;
                                 }
                             if (this._bufferService.cols - u > 1) {
-                                const T = this._getJoinedRanges(v, _, p, e, u);
-                                for (let x = 0; x < T.length; x++)
-                                    h.push(T[x]);
+                                const B = this._getJoinedRanges(g, _, S, t, u);
+                                for (let T = 0; T < B.length; T++)
+                                    h.push(B[T]);
                             }
                             return h;
                         }
-                        _getJoinedRanges(t, e, h, v, u) {
-                            const p = t.substring(e, h);
+                        _getJoinedRanges(e, t, h, g, u) {
+                            const S = e.substring(t, h);
                             let _ = [];
                             try {
-                                _ = this._characterJoiners[0].handler(p);
+                                _ = this._characterJoiners[0].handler(S);
                             } catch (b) {
                                 console.error(b);
                             }
                             for (let b = 1; b < this._characterJoiners.length; b++)
                                 try {
-                                    const A = this._characterJoiners[b].handler(p);
-                                    for (let T = 0; T < A.length; T++)
-                                        jt._mergeRanges(_, A[T]);
-                                } catch (A) {
-                                    console.error(A);
+                                    const R = this._characterJoiners[b].handler(S);
+                                    for (let B = 0; B < R.length; B++)
+                                        jt._mergeRanges(_, R[B]);
+                                } catch (R) {
+                                    console.error(R);
                                 }
-                            return this._stringRangesToCellRanges(_, v, u), _;
+                            return this._stringRangesToCellRanges(_, g, u), _;
                         }
-                        _stringRangesToCellRanges(t, e, h) {
-                            let v = 0,
+                        _stringRangesToCellRanges(e, t, h) {
+                            let g = 0,
                                 u = !1,
-                                p = 0,
-                                _ = t[v];
+                                S = 0,
+                                _ = e[g];
                             if (_) {
                                 for (let b = h; b < this._bufferService.cols; b++) {
-                                    const A = e.getWidth(b),
-                                        T = e.getString(b).length || d.WHITESPACE_CELL_CHAR.length;
-                                    if (A !== 0) {
-                                        if (!u && _[0] <= p && (_[0] = b, u = !0), _[1] <= p) {
-                                            if (_[1] = b, _ = t[++v], !_)
+                                    const R = t.getWidth(b),
+                                        B = t.getString(b).length || d.WHITESPACE_CELL_CHAR.length;
+                                    if (R !== 0) {
+                                        if (!u && _[0] <= S && (_[0] = b, u = !0), _[1] <= S) {
+                                            if (_[1] = b, _ = e[++g], !_)
                                                 break;
-                                            _[0] <= p ? (_[0] = b, u = !0) : u = !1;
+                                            _[0] <= S ? (_[0] = b, u = !0) : u = !1;
                                         }
-                                        p += T;
+                                        S += B;
                                     }
                                 }
                                 _ && (_[1] = this._bufferService.cols);
                             }
                         }
-                        static _mergeRanges(t, e) {
+                        static _mergeRanges(e, t) {
                             let h = !1;
-                            for (let v = 0; v < t.length; v++) {
-                                const u = t[v];
+                            for (let g = 0; g < e.length; g++) {
+                                const u = e[g];
                                 if (h) {
-                                    if (e[1] <= u[0])
-                                        return t[v - 1][1] = e[1], t;
-                                    if (e[1] <= u[1])
-                                        return t[v - 1][1] = Math.max(e[1], u[1]), t.splice(v, 1), t;
-                                    t.splice(v, 1), v--;
+                                    if (t[1] <= u[0])
+                                        return e[g - 1][1] = t[1], e;
+                                    if (t[1] <= u[1])
+                                        return e[g - 1][1] = Math.max(t[1], u[1]), e.splice(g, 1), e;
+                                    e.splice(g, 1), g--;
                                 } else {
-                                    if (e[1] <= u[0])
-                                        return t.splice(v, 0, e), t;
-                                    if (e[1] <= u[1])
-                                        return u[0] = Math.min(e[0], u[0]), t;
-                                    e[0] < u[1] && (u[0] = Math.min(e[0], u[0]), h = !0);
+                                    if (t[1] <= u[0])
+                                        return e.splice(g, 0, t), e;
+                                    if (t[1] <= u[1])
+                                        return u[0] = Math.min(t[0], u[0]), e;
+                                    t[0] < u[1] && (u[0] = Math.min(t[0], u[0]), h = !0);
                                 }
                             }
-                            return h ? t[t.length - 1][1] = e[1] : t.push(e), t;
+                            return h ? e[e.length - 1][1] = t[1] : e.push(t), e;
                         }
                     };
-                    i.CharacterJoinerService = s = o([c(0, g.IBufferService)], s);
+                    i.CharacterJoinerService = s = o([c(0, m.IBufferService)], s);
                 },
                 5114: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CoreBrowserService = void 0;
                     const o = n(844),
                         c = n(8460),
                         a = n(3656);
                     class d extends o.Disposable {
                         constructor(l, s, r) {
-                            super(), this._textarea = l, this._window = s, this.mainDocument = r, this._isFocused = !1, this._cachedIsFocused = void 0, this._screenDprMonitor = new f(this._window), this._onDprChange = this.register(new c.EventEmitter()), this.onDprChange = this._onDprChange.event, this._onWindowChange = this.register(new c.EventEmitter()), this.onWindowChange = this._onWindowChange.event, this.register(this.onWindowChange((t) => this._screenDprMonitor.setWindow(t))), this.register((0, c.forwardEvent)(this._screenDprMonitor.onDprChange, this._onDprChange)), this._textarea.addEventListener("focus", () => this._isFocused = !0), this._textarea.addEventListener("blur", () => this._isFocused = !1);
+                            super(), this._textarea = l, this._window = s, this.mainDocument = r, this._isFocused = !1, this._cachedIsFocused = void 0, this._screenDprMonitor = new v(this._window), this._onDprChange = this.register(new c.EventEmitter()), this.onDprChange = this._onDprChange.event, this._onWindowChange = this.register(new c.EventEmitter()), this.onWindowChange = this._onWindowChange.event, this.register(this.onWindowChange((e) => this._screenDprMonitor.setWindow(e))), this.register((0, c.forwardEvent)(this._screenDprMonitor.onDprChange, this._onDprChange)), this._textarea.addEventListener("focus", () => this._isFocused = !0), this._textarea.addEventListener("blur", () => this._isFocused = !1);
                         }
                         get window() {
                             return this._window;
                         }
                         set window(l) {
                             this._window !== l && (this._window = l, this._onWindowChange.fire(this._window));
                         }
@@ -4725,15 +4725,15 @@
                             return this.window.devicePixelRatio;
                         }
                         get isFocused() {
                             return this._cachedIsFocused === void 0 && (this._cachedIsFocused = this._isFocused && this._textarea.ownerDocument.hasFocus(), queueMicrotask(() => this._cachedIsFocused = void 0)), this._cachedIsFocused;
                         }
                     }
                     i.CoreBrowserService = d;
-                    class f extends o.Disposable {
+                    class v extends o.Disposable {
                         constructor(l) {
                             super(), this._parentWindow = l, this._windowResizeListener = this.register(new o.MutableDisposable()), this._onDprChange = this.register(new c.EventEmitter()), this.onDprChange = this._onDprChange.event, this._outerListener = () => this._setDprAndFireIfDiffers(), this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this._updateDpr(), this._setWindowResizeListener(), this.register((0, o.toDisposable)(() => this.clearListener()));
                         }
                         setWindow(l) {
                             this._parentWindow = l, this._setWindowResizeListener(), this._setDprAndFireIfDiffers();
                         }
                         _setWindowResizeListener() {
@@ -4759,224 +4759,224 @@
                     class c extends o.Disposable {
                         constructor() {
                             super(), this.linkProviders = [], this.register((0, o.toDisposable)(() => this.linkProviders.length = 0));
                         }
                         registerLinkProvider(d) {
                             return this.linkProviders.push(d), {
                                 dispose: () => {
-                                    const f = this.linkProviders.indexOf(d);
-                                    f !== -1 && this.linkProviders.splice(f, 1);
+                                    const v = this.linkProviders.indexOf(d);
+                                    v !== -1 && this.linkProviders.splice(v, 1);
                                 }
                             };
                         }
                     }
                     i.LinkProviderService = c;
                 },
                 8934: function(k, i, n) {
-                    var o = this && this.__decorate || function(g, l, s, r) {
-                            var t, e = arguments.length,
-                                h = e < 3 ? l : r === null ? r = Object.getOwnPropertyDescriptor(l, s) : r;
+                    var o = this && this.__decorate || function(m, l, s, r) {
+                            var e, t = arguments.length,
+                                h = t < 3 ? l : r === null ? r = Object.getOwnPropertyDescriptor(l, s) : r;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                h = Reflect.decorate(g, l, s, r);
+                                h = Reflect.decorate(m, l, s, r);
                             else
-                                for (var v = g.length - 1; v >= 0; v--)
-                                    (t = g[v]) && (h = (e < 3 ? t(h) : e > 3 ? t(l, s, h) : t(l, s)) || h);
-                            return e > 3 && h && Object.defineProperty(l, s, h), h;
+                                for (var g = m.length - 1; g >= 0; g--)
+                                    (e = m[g]) && (h = (t < 3 ? e(h) : t > 3 ? e(l, s, h) : e(l, s)) || h);
+                            return t > 3 && h && Object.defineProperty(l, s, h), h;
                         },
-                        c = this && this.__param || function(g, l) {
+                        c = this && this.__param || function(m, l) {
                             return function(s, r) {
-                                l(s, r, g);
+                                l(s, r, m);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.MouseService = void 0;
                     const a = n(4725),
                         d = n(9806);
-                    let f = i.MouseService = class {
-                        constructor(g, l) {
-                            this._renderService = g, this._charSizeService = l;
+                    let v = i.MouseService = class {
+                        constructor(m, l) {
+                            this._renderService = m, this._charSizeService = l;
                         }
-                        getCoords(g, l, s, r, t) {
-                            return (0, d.getCoords)(window, g, l, s, r, this._charSizeService.hasValidSize, this._renderService.dimensions.css.cell.width, this._renderService.dimensions.css.cell.height, t);
+                        getCoords(m, l, s, r, e) {
+                            return (0, d.getCoords)(window, m, l, s, r, this._charSizeService.hasValidSize, this._renderService.dimensions.css.cell.width, this._renderService.dimensions.css.cell.height, e);
                         }
-                        getMouseReportCoords(g, l) {
-                            const s = (0, d.getCoordsRelativeToElement)(window, g, l);
+                        getMouseReportCoords(m, l) {
+                            const s = (0, d.getCoordsRelativeToElement)(window, m, l);
                             if (this._charSizeService.hasValidSize)
                                 return s[0] = Math.min(Math.max(s[0], 0), this._renderService.dimensions.css.canvas.width - 1), s[1] = Math.min(Math.max(s[1], 0), this._renderService.dimensions.css.canvas.height - 1), {
                                     col: Math.floor(s[0] / this._renderService.dimensions.css.cell.width),
                                     row: Math.floor(s[1] / this._renderService.dimensions.css.cell.height),
                                     x: Math.floor(s[0]),
                                     y: Math.floor(s[1])
                                 };
                         }
                     };
-                    i.MouseService = f = o([c(0, a.IRenderService), c(1, a.ICharSizeService)], f);
+                    i.MouseService = v = o([c(0, a.IRenderService), c(1, a.ICharSizeService)], v);
                 },
                 3230: function(k, i, n) {
-                    var o = this && this.__decorate || function(t, e, h, v) {
-                            var u, p = arguments.length,
-                                _ = p < 3 ? e : v === null ? v = Object.getOwnPropertyDescriptor(e, h) : v;
+                    var o = this && this.__decorate || function(e, t, h, g) {
+                            var u, S = arguments.length,
+                                _ = S < 3 ? t : g === null ? g = Object.getOwnPropertyDescriptor(t, h) : g;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                _ = Reflect.decorate(t, e, h, v);
+                                _ = Reflect.decorate(e, t, h, g);
                             else
-                                for (var b = t.length - 1; b >= 0; b--)
-                                    (u = t[b]) && (_ = (p < 3 ? u(_) : p > 3 ? u(e, h, _) : u(e, h)) || _);
-                            return p > 3 && _ && Object.defineProperty(e, h, _), _;
+                                for (var b = e.length - 1; b >= 0; b--)
+                                    (u = e[b]) && (_ = (S < 3 ? u(_) : S > 3 ? u(t, h, _) : u(t, h)) || _);
+                            return S > 3 && _ && Object.defineProperty(t, h, _), _;
                         },
-                        c = this && this.__param || function(t, e) {
-                            return function(h, v) {
-                                e(h, v, t);
+                        c = this && this.__param || function(e, t) {
+                            return function(h, g) {
+                                t(h, g, e);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.RenderService = void 0;
                     const a = n(6193),
                         d = n(4725),
-                        f = n(8460),
-                        g = n(844),
+                        v = n(8460),
+                        m = n(844),
                         l = n(7226),
                         s = n(2585);
-                    let r = i.RenderService = class extends g.Disposable {
+                    let r = i.RenderService = class extends m.Disposable {
                         get dimensions() {
                             return this._renderer.value.dimensions;
                         }
-                        constructor(t, e, h, v, u, p, _, b) {
-                            super(), this._rowCount = t, this._charSizeService = v, this._renderer = this.register(new g.MutableDisposable()), this._pausedResizeTask = new l.DebouncedIdleTask(), this._observerDisposable = this.register(new g.MutableDisposable()), this._isPaused = !1, this._needsFullRefresh = !1, this._isNextRenderRedrawOnly = !0, this._needsSelectionRefresh = !1, this._canvasWidth = 0, this._canvasHeight = 0, this._selectionState = {
+                        constructor(e, t, h, g, u, S, _, b) {
+                            super(), this._rowCount = e, this._charSizeService = g, this._renderer = this.register(new m.MutableDisposable()), this._pausedResizeTask = new l.DebouncedIdleTask(), this._observerDisposable = this.register(new m.MutableDisposable()), this._isPaused = !1, this._needsFullRefresh = !1, this._isNextRenderRedrawOnly = !0, this._needsSelectionRefresh = !1, this._canvasWidth = 0, this._canvasHeight = 0, this._selectionState = {
                                 start: void 0,
                                 end: void 0,
                                 columnSelectMode: !1
-                            }, this._onDimensionsChange = this.register(new f.EventEmitter()), this.onDimensionsChange = this._onDimensionsChange.event, this._onRenderedViewportChange = this.register(new f.EventEmitter()), this.onRenderedViewportChange = this._onRenderedViewportChange.event, this._onRender = this.register(new f.EventEmitter()), this.onRender = this._onRender.event, this._onRefreshRequest = this.register(new f.EventEmitter()), this.onRefreshRequest = this._onRefreshRequest.event, this._renderDebouncer = new a.RenderDebouncer((A, T) => this._renderRows(A, T), _), this.register(this._renderDebouncer), this.register(_.onDprChange(() => this.handleDevicePixelRatioChange())), this.register(p.onResize(() => this._fullRefresh())), this.register(p.buffers.onBufferActivate(() => {
-                                var A;
-                                return (A = this._renderer.value) == null ? void 0 : A.clear();
+                            }, this._onDimensionsChange = this.register(new v.EventEmitter()), this.onDimensionsChange = this._onDimensionsChange.event, this._onRenderedViewportChange = this.register(new v.EventEmitter()), this.onRenderedViewportChange = this._onRenderedViewportChange.event, this._onRender = this.register(new v.EventEmitter()), this.onRender = this._onRender.event, this._onRefreshRequest = this.register(new v.EventEmitter()), this.onRefreshRequest = this._onRefreshRequest.event, this._renderDebouncer = new a.RenderDebouncer((R, B) => this._renderRows(R, B), _), this.register(this._renderDebouncer), this.register(_.onDprChange(() => this.handleDevicePixelRatioChange())), this.register(S.onResize(() => this._fullRefresh())), this.register(S.buffers.onBufferActivate(() => {
+                                var R;
+                                return (R = this._renderer.value) == null ? void 0 : R.clear();
                             })), this.register(h.onOptionChange(() => this._handleOptionsChanged())), this.register(this._charSizeService.onCharSizeChange(() => this.handleCharSizeChanged())), this.register(u.onDecorationRegistered(() => this._fullRefresh())), this.register(u.onDecorationRemoved(() => this._fullRefresh())), this.register(h.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio", "rescaleOverlappingGlyphs"], () => {
-                                this.clear(), this.handleResize(p.cols, p.rows), this._fullRefresh();
-                            })), this.register(h.onMultipleOptionChange(["cursorBlink", "cursorStyle"], () => this.refreshRows(p.buffer.y, p.buffer.y, !0))), this.register(b.onChangeColors(() => this._fullRefresh())), this._registerIntersectionObserver(_.window, e), this.register(_.onWindowChange((A) => this._registerIntersectionObserver(A, e)));
+                                this.clear(), this.handleResize(S.cols, S.rows), this._fullRefresh();
+                            })), this.register(h.onMultipleOptionChange(["cursorBlink", "cursorStyle"], () => this.refreshRows(S.buffer.y, S.buffer.y, !0))), this.register(b.onChangeColors(() => this._fullRefresh())), this._registerIntersectionObserver(_.window, t), this.register(_.onWindowChange((R) => this._registerIntersectionObserver(R, t)));
                         }
-                        _registerIntersectionObserver(t, e) {
-                            if ("IntersectionObserver" in t) {
-                                const h = new t.IntersectionObserver((v) => this._handleIntersectionChange(v[v.length - 1]), {
+                        _registerIntersectionObserver(e, t) {
+                            if ("IntersectionObserver" in e) {
+                                const h = new e.IntersectionObserver((g) => this._handleIntersectionChange(g[g.length - 1]), {
                                     threshold: 0
                                 });
-                                h.observe(e), this._observerDisposable.value = (0, g.toDisposable)(() => h.disconnect());
+                                h.observe(t), this._observerDisposable.value = (0, m.toDisposable)(() => h.disconnect());
                             }
                         }
-                        _handleIntersectionChange(t) {
-                            this._isPaused = t.isIntersecting === void 0 ? t.intersectionRatio === 0 : !t.isIntersecting, this._isPaused || this._charSizeService.hasValidSize || this._charSizeService.measure(), !this._isPaused && this._needsFullRefresh && (this._pausedResizeTask.flush(), this.refreshRows(0, this._rowCount - 1), this._needsFullRefresh = !1);
+                        _handleIntersectionChange(e) {
+                            this._isPaused = e.isIntersecting === void 0 ? e.intersectionRatio === 0 : !e.isIntersecting, this._isPaused || this._charSizeService.hasValidSize || this._charSizeService.measure(), !this._isPaused && this._needsFullRefresh && (this._pausedResizeTask.flush(), this.refreshRows(0, this._rowCount - 1), this._needsFullRefresh = !1);
                         }
-                        refreshRows(t, e, h = !1) {
-                            this._isPaused ? this._needsFullRefresh = !0 : (h || (this._isNextRenderRedrawOnly = !1), this._renderDebouncer.refresh(t, e, this._rowCount));
+                        refreshRows(e, t, h = !1) {
+                            this._isPaused ? this._needsFullRefresh = !0 : (h || (this._isNextRenderRedrawOnly = !1), this._renderDebouncer.refresh(e, t, this._rowCount));
                         }
-                        _renderRows(t, e) {
-                            this._renderer.value && (t = Math.min(t, this._rowCount - 1), e = Math.min(e, this._rowCount - 1), this._renderer.value.renderRows(t, e), this._needsSelectionRefresh && (this._renderer.value.handleSelectionChanged(this._selectionState.start, this._selectionState.end, this._selectionState.columnSelectMode), this._needsSelectionRefresh = !1), this._isNextRenderRedrawOnly || this._onRenderedViewportChange.fire({
-                                start: t,
-                                end: e
+                        _renderRows(e, t) {
+                            this._renderer.value && (e = Math.min(e, this._rowCount - 1), t = Math.min(t, this._rowCount - 1), this._renderer.value.renderRows(e, t), this._needsSelectionRefresh && (this._renderer.value.handleSelectionChanged(this._selectionState.start, this._selectionState.end, this._selectionState.columnSelectMode), this._needsSelectionRefresh = !1), this._isNextRenderRedrawOnly || this._onRenderedViewportChange.fire({
+                                start: e,
+                                end: t
                             }), this._onRender.fire({
-                                start: t,
-                                end: e
+                                start: e,
+                                end: t
                             }), this._isNextRenderRedrawOnly = !0);
                         }
-                        resize(t, e) {
-                            this._rowCount = e, this._fireOnCanvasResize();
+                        resize(e, t) {
+                            this._rowCount = t, this._fireOnCanvasResize();
                         }
                         _handleOptionsChanged() {
                             this._renderer.value && (this.refreshRows(0, this._rowCount - 1), this._fireOnCanvasResize());
                         }
                         _fireOnCanvasResize() {
                             this._renderer.value && (this._renderer.value.dimensions.css.canvas.width === this._canvasWidth && this._renderer.value.dimensions.css.canvas.height === this._canvasHeight || this._onDimensionsChange.fire(this._renderer.value.dimensions));
                         }
                         hasRenderer() {
                             return !!this._renderer.value;
                         }
-                        setRenderer(t) {
-                            this._renderer.value = t, this._renderer.value && (this._renderer.value.onRequestRedraw((e) => this.refreshRows(e.start, e.end, !0)), this._needsSelectionRefresh = !0, this._fullRefresh());
+                        setRenderer(e) {
+                            this._renderer.value = e, this._renderer.value && (this._renderer.value.onRequestRedraw((t) => this.refreshRows(t.start, t.end, !0)), this._needsSelectionRefresh = !0, this._fullRefresh());
                         }
-                        addRefreshCallback(t) {
-                            return this._renderDebouncer.addRefreshCallback(t);
+                        addRefreshCallback(e) {
+                            return this._renderDebouncer.addRefreshCallback(e);
                         }
                         _fullRefresh() {
                             this._isPaused ? this._needsFullRefresh = !0 : this.refreshRows(0, this._rowCount - 1);
                         }
                         clearTextureAtlas() {
-                            var t, e;
-                            this._renderer.value && ((e = (t = this._renderer.value).clearTextureAtlas) == null || e.call(t), this._fullRefresh());
+                            var e, t;
+                            this._renderer.value && ((t = (e = this._renderer.value).clearTextureAtlas) == null || t.call(e), this._fullRefresh());
                         }
                         handleDevicePixelRatioChange() {
                             this._charSizeService.measure(), this._renderer.value && (this._renderer.value.handleDevicePixelRatioChange(), this.refreshRows(0, this._rowCount - 1));
                         }
-                        handleResize(t, e) {
+                        handleResize(e, t) {
                             this._renderer.value && (this._isPaused ? this._pausedResizeTask.set(() => {
                                 var h;
-                                return (h = this._renderer.value) == null ? void 0 : h.handleResize(t, e);
-                            }) : this._renderer.value.handleResize(t, e), this._fullRefresh());
+                                return (h = this._renderer.value) == null ? void 0 : h.handleResize(e, t);
+                            }) : this._renderer.value.handleResize(e, t), this._fullRefresh());
                         }
                         handleCharSizeChanged() {
-                            var t;
-                            (t = this._renderer.value) == null || t.handleCharSizeChanged();
+                            var e;
+                            (e = this._renderer.value) == null || e.handleCharSizeChanged();
                         }
                         handleBlur() {
-                            var t;
-                            (t = this._renderer.value) == null || t.handleBlur();
+                            var e;
+                            (e = this._renderer.value) == null || e.handleBlur();
                         }
                         handleFocus() {
-                            var t;
-                            (t = this._renderer.value) == null || t.handleFocus();
+                            var e;
+                            (e = this._renderer.value) == null || e.handleFocus();
                         }
-                        handleSelectionChanged(t, e, h) {
-                            var v;
-                            this._selectionState.start = t, this._selectionState.end = e, this._selectionState.columnSelectMode = h, (v = this._renderer.value) == null || v.handleSelectionChanged(t, e, h);
+                        handleSelectionChanged(e, t, h) {
+                            var g;
+                            this._selectionState.start = e, this._selectionState.end = t, this._selectionState.columnSelectMode = h, (g = this._renderer.value) == null || g.handleSelectionChanged(e, t, h);
                         }
                         handleCursorMove() {
-                            var t;
-                            (t = this._renderer.value) == null || t.handleCursorMove();
+                            var e;
+                            (e = this._renderer.value) == null || e.handleCursorMove();
                         }
                         clear() {
-                            var t;
-                            (t = this._renderer.value) == null || t.clear();
+                            var e;
+                            (e = this._renderer.value) == null || e.clear();
                         }
                     };
                     i.RenderService = r = o([c(2, s.IOptionsService), c(3, d.ICharSizeService), c(4, s.IDecorationService), c(5, s.IBufferService), c(6, d.ICoreBrowserService), c(7, d.IThemeService)], r);
                 },
                 9312: function(k, i, n) {
-                    var o = this && this.__decorate || function(_, b, A, T) {
-                            var x, L = arguments.length,
-                                H = L < 3 ? b : T === null ? T = Object.getOwnPropertyDescriptor(b, A) : T;
+                    var o = this && this.__decorate || function(_, b, R, B) {
+                            var T, L = arguments.length,
+                                H = L < 3 ? b : B === null ? B = Object.getOwnPropertyDescriptor(b, R) : B;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                H = Reflect.decorate(_, b, A, T);
+                                H = Reflect.decorate(_, b, R, B);
                             else
                                 for (var W = _.length - 1; W >= 0; W--)
-                                    (x = _[W]) && (H = (L < 3 ? x(H) : L > 3 ? x(b, A, H) : x(b, A)) || H);
-                            return L > 3 && H && Object.defineProperty(b, A, H), H;
+                                    (T = _[W]) && (H = (L < 3 ? T(H) : L > 3 ? T(b, R, H) : T(b, R)) || H);
+                            return L > 3 && H && Object.defineProperty(b, R, H), H;
                         },
                         c = this && this.__param || function(_, b) {
-                            return function(A, T) {
-                                b(A, T, _);
+                            return function(R, B) {
+                                b(R, B, _);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.SelectionService = void 0;
                     const a = n(9806),
                         d = n(9504),
-                        f = n(456),
-                        g = n(4725),
+                        v = n(456),
+                        m = n(4725),
                         l = n(8460),
                         s = n(844),
                         r = n(6114),
-                        t = n(4841),
-                        e = n(511),
+                        e = n(4841),
+                        t = n(511),
                         h = n(2585),
-                        v = " ",
-                        u = new RegExp(v, "g");
-                    let p = i.SelectionService = class extends s.Disposable {
-                        constructor(_, b, A, T, x, L, H, W, U) {
-                            super(), this._element = _, this._screenElement = b, this._linkifier = A, this._bufferService = T, this._coreService = x, this._mouseService = L, this._optionsService = H, this._renderService = W, this._coreBrowserService = U, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new e.CellData(), this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new l.EventEmitter()), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new l.EventEmitter()), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new l.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new l.EventEmitter()), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = (K) => this._handleMouseMove(K), this._mouseUpListener = (K) => this._handleMouseUp(K), this._coreService.onUserInput(() => {
+                        g = " ",
+                        u = new RegExp(g, "g");
+                    let S = i.SelectionService = class extends s.Disposable {
+                        constructor(_, b, R, B, T, L, H, W, j) {
+                            super(), this._element = _, this._screenElement = b, this._linkifier = R, this._bufferService = B, this._coreService = T, this._mouseService = L, this._optionsService = H, this._renderService = W, this._coreBrowserService = j, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new t.CellData(), this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new l.EventEmitter()), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new l.EventEmitter()), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new l.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new l.EventEmitter()), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = (V) => this._handleMouseMove(V), this._mouseUpListener = (V) => this._handleMouseUp(V), this._coreService.onUserInput(() => {
                                 this.hasSelection && this.clearSelection();
-                            }), this._trimListener = this._bufferService.buffer.lines.onTrim((K) => this._handleTrim(K)), this.register(this._bufferService.buffers.onBufferActivate((K) => this._handleBufferActivate(K))), this.enable(), this._model = new f.SelectionModel(this._bufferService), this._activeSelectionMode = 0, this.register((0, s.toDisposable)(() => {
+                            }), this._trimListener = this._bufferService.buffer.lines.onTrim((V) => this._handleTrim(V)), this.register(this._bufferService.buffers.onBufferActivate((V) => this._handleBufferActivate(V))), this.enable(), this._model = new v.SelectionModel(this._bufferService), this._activeSelectionMode = 0, this.register((0, s.toDisposable)(() => {
                                 this._removeMouseDownListeners();
                             }));
                         }
                         reset() {
                             this.clearSelection();
                         }
                         disable() {
@@ -4997,40 +4997,40 @@
                             return !(!_ || !b || _[0] === b[0] && _[1] === b[1]);
                         }
                         get selectionText() {
                             const _ = this._model.finalSelectionStart,
                                 b = this._model.finalSelectionEnd;
                             if (!_ || !b)
                                 return "";
-                            const A = this._bufferService.buffer,
-                                T = [];
+                            const R = this._bufferService.buffer,
+                                B = [];
                             if (this._activeSelectionMode === 3) {
                                 if (_[0] === b[0])
                                     return "";
-                                const x = _[0] < b[0] ? _[0] : b[0],
+                                const T = _[0] < b[0] ? _[0] : b[0],
                                     L = _[0] < b[0] ? b[0] : _[0];
                                 for (let H = _[1]; H <= b[1]; H++) {
-                                    const W = A.translateBufferLineToString(H, !0, x, L);
-                                    T.push(W);
+                                    const W = R.translateBufferLineToString(H, !0, T, L);
+                                    B.push(W);
                                 }
                             } else {
-                                const x = _[1] === b[1] ? b[0] : void 0;
-                                T.push(A.translateBufferLineToString(_[1], !0, _[0], x));
+                                const T = _[1] === b[1] ? b[0] : void 0;
+                                B.push(R.translateBufferLineToString(_[1], !0, _[0], T));
                                 for (let L = _[1] + 1; L <= b[1] - 1; L++) {
-                                    const H = A.lines.get(L),
-                                        W = A.translateBufferLineToString(L, !0);
-                                    H != null && H.isWrapped ? T[T.length - 1] += W : T.push(W);
+                                    const H = R.lines.get(L),
+                                        W = R.translateBufferLineToString(L, !0);
+                                    H != null && H.isWrapped ? B[B.length - 1] += W : B.push(W);
                                 }
                                 if (_[1] !== b[1]) {
-                                    const L = A.lines.get(b[1]),
-                                        H = A.translateBufferLineToString(b[1], !0, 0, b[0]);
-                                    L && L.isWrapped ? T[T.length - 1] += H : T.push(H);
+                                    const L = R.lines.get(b[1]),
+                                        H = R.translateBufferLineToString(b[1], !0, 0, b[0]);
+                                    L && L.isWrapped ? B[B.length - 1] += H : B.push(H);
                                 }
                             }
-                            return T.map((x) => x.replace(u, " ")).join(r.isWindows ? `\r
+                            return B.map((T) => T.replace(u, " ")).join(r.isWindows ? `\r
 ` : `
 `);
                         }
                         clearSelection() {
                             this._model.clearSelection(), this._removeMouseDownListeners(), this.refresh(), this._onSelectionChange.fire();
                         }
                         refresh(_) {
@@ -5041,33 +5041,33 @@
                                 start: this._model.finalSelectionStart,
                                 end: this._model.finalSelectionEnd,
                                 columnSelectMode: this._activeSelectionMode === 3
                             });
                         }
                         _isClickInSelection(_) {
                             const b = this._getMouseBufferCoords(_),
-                                A = this._model.finalSelectionStart,
-                                T = this._model.finalSelectionEnd;
-                            return !!(A && T && b) && this._areCoordsInSelection(b, A, T);
+                                R = this._model.finalSelectionStart,
+                                B = this._model.finalSelectionEnd;
+                            return !!(R && B && b) && this._areCoordsInSelection(b, R, B);
                         }
                         isCellInSelection(_, b) {
-                            const A = this._model.finalSelectionStart,
-                                T = this._model.finalSelectionEnd;
-                            return !(!A || !T) && this._areCoordsInSelection([_, b], A, T);
+                            const R = this._model.finalSelectionStart,
+                                B = this._model.finalSelectionEnd;
+                            return !(!R || !B) && this._areCoordsInSelection([_, b], R, B);
                         }
-                        _areCoordsInSelection(_, b, A) {
-                            return _[1] > b[1] && _[1] < A[1] || b[1] === A[1] && _[1] === b[1] && _[0] >= b[0] && _[0] < A[0] || b[1] < A[1] && _[1] === A[1] && _[0] < A[0] || b[1] < A[1] && _[1] === b[1] && _[0] >= b[0];
+                        _areCoordsInSelection(_, b, R) {
+                            return _[1] > b[1] && _[1] < R[1] || b[1] === R[1] && _[1] === b[1] && _[0] >= b[0] && _[0] < R[0] || b[1] < R[1] && _[1] === R[1] && _[0] < R[0] || b[1] < R[1] && _[1] === b[1] && _[0] >= b[0];
                         }
                         _selectWordAtCursor(_, b) {
-                            var x, L;
-                            const A = (L = (x = this._linkifier.currentLink) == null ? void 0 : x.link) == null ? void 0 : L.range;
-                            if (A)
-                                return this._model.selectionStart = [A.start.x - 1, A.start.y - 1], this._model.selectionStartLength = (0, t.getRangeLength)(A, this._bufferService.cols), this._model.selectionEnd = void 0, !0;
-                            const T = this._getMouseBufferCoords(_);
-                            return !!T && (this._selectWordAt(T, b), this._model.selectionEnd = void 0, !0);
+                            var T, L;
+                            const R = (L = (T = this._linkifier.currentLink) == null ? void 0 : T.link) == null ? void 0 : L.range;
+                            if (R)
+                                return this._model.selectionStart = [R.start.x - 1, R.start.y - 1], this._model.selectionStartLength = (0, e.getRangeLength)(R, this._bufferService.cols), this._model.selectionEnd = void 0, !0;
+                            const B = this._getMouseBufferCoords(_);
+                            return !!B && (this._selectWordAt(B, b), this._model.selectionEnd = void 0, !0);
                         }
                         selectAll() {
                             this._model.isSelectAllActive = !0, this.refresh(), this._onSelectionChange.fire();
                         }
                         selectLines(_, b) {
                             this._model.clearSelection(), _ = Math.max(_, 0), b = Math.min(b, this._bufferService.buffer.lines.length - 1), this._model.selectionStart = [0, _], this._model.selectionEnd = [this._bufferService.cols, b], this.refresh(), this._onSelectionChange.fire();
                         }
@@ -5077,16 +5077,16 @@
                         _getMouseBufferCoords(_) {
                             const b = this._mouseService.getCoords(_, this._screenElement, this._bufferService.cols, this._bufferService.rows, !0);
                             if (b)
                                 return b[0]--, b[1]--, b[1] += this._bufferService.buffer.ydisp, b;
                         }
                         _getMouseEventScrollAmount(_) {
                             let b = (0, a.getCoordsRelativeToElement)(this._coreBrowserService.window, _, this._screenElement)[1];
-                            const A = this._renderService.dimensions.css.canvas.height;
-                            return b >= 0 && b <= A ? 0 : (b > A && (b -= A), b = Math.min(Math.max(b, -50), 50), b /= 50, b / Math.abs(b) + Math.round(14 * b));
+                            const R = this._renderService.dimensions.css.canvas.height;
+                            return b >= 0 && b <= R ? 0 : (b > R && (b -= R), b = Math.min(Math.max(b, -50), 50), b /= 50, b / Math.abs(b) + Math.round(14 * b));
                         }
                         shouldForceSelection(_) {
                             return r.isMac ? _.altKey && this._optionsService.rawOptions.macOptionClickForcesSelection : _.shiftKey;
                         }
                         handleMouseDown(_) {
                             if (this._mouseDownTimeStamp = _.timeStamp, (_.button !== 2 || !this.hasSelection) && _.button === 0) {
                                 if (!this._enabled) {
@@ -5126,18 +5126,18 @@
                         _handleMouseMove(_) {
                             if (_.stopImmediatePropagation(), !this._model.selectionStart)
                                 return;
                             const b = this._model.selectionEnd ? [this._model.selectionEnd[0], this._model.selectionEnd[1]] : null;
                             if (this._model.selectionEnd = this._getMouseBufferCoords(_), !this._model.selectionEnd)
                                 return void this.refresh(!0);
                             this._activeSelectionMode === 2 ? this._model.selectionEnd[1] < this._model.selectionStart[1] ? this._model.selectionEnd[0] = 0 : this._model.selectionEnd[0] = this._bufferService.cols : this._activeSelectionMode === 1 && this._selectToWordAt(this._model.selectionEnd), this._dragScrollAmount = this._getMouseEventScrollAmount(_), this._activeSelectionMode !== 3 && (this._dragScrollAmount > 0 ? this._model.selectionEnd[0] = this._bufferService.cols : this._dragScrollAmount < 0 && (this._model.selectionEnd[0] = 0));
-                            const A = this._bufferService.buffer;
-                            if (this._model.selectionEnd[1] < A.lines.length) {
-                                const T = A.lines.get(this._model.selectionEnd[1]);
-                                T && T.hasWidth(this._model.selectionEnd[0]) === 0 && this._model.selectionEnd[0] < this._bufferService.cols && this._model.selectionEnd[0]++;
+                            const R = this._bufferService.buffer;
+                            if (this._model.selectionEnd[1] < R.lines.length) {
+                                const B = R.lines.get(this._model.selectionEnd[1]);
+                                B && B.hasWidth(this._model.selectionEnd[0]) === 0 && this._model.selectionEnd[0] < this._bufferService.cols && this._model.selectionEnd[0]++;
                             }
                             b && b[0] === this._model.selectionEnd[0] && b[1] === this._model.selectionEnd[1] || this.refresh(!0);
                         }
                         _dragScroll() {
                             if (this._model.selectionEnd && this._model.selectionStart && this._dragScrollAmount) {
                                 this._onRequestScrollLines.fire({
                                     amount: this._dragScrollAmount,
@@ -5147,380 +5147,380 @@
                                 this._dragScrollAmount > 0 ? (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = this._bufferService.cols), this._model.selectionEnd[1] = Math.min(_.ydisp + this._bufferService.rows, _.lines.length - 1)) : (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = 0), this._model.selectionEnd[1] = _.ydisp), this.refresh();
                             }
                         }
                         _handleMouseUp(_) {
                             const b = _.timeStamp - this._mouseDownTimeStamp;
                             if (this._removeMouseDownListeners(), this.selectionText.length <= 1 && b < 500 && _.altKey && this._optionsService.rawOptions.altClickMovesCursor) {
                                 if (this._bufferService.buffer.ybase === this._bufferService.buffer.ydisp) {
-                                    const A = this._mouseService.getCoords(_, this._element, this._bufferService.cols, this._bufferService.rows, !1);
-                                    if (A && A[0] !== void 0 && A[1] !== void 0) {
-                                        const T = (0, d.moveToCellSequence)(A[0] - 1, A[1] - 1, this._bufferService, this._coreService.decPrivateModes.applicationCursorKeys);
-                                        this._coreService.triggerDataEvent(T, !0);
+                                    const R = this._mouseService.getCoords(_, this._element, this._bufferService.cols, this._bufferService.rows, !1);
+                                    if (R && R[0] !== void 0 && R[1] !== void 0) {
+                                        const B = (0, d.moveToCellSequence)(R[0] - 1, R[1] - 1, this._bufferService, this._coreService.decPrivateModes.applicationCursorKeys);
+                                        this._coreService.triggerDataEvent(B, !0);
                                     }
                                 }
                             } else
                                 this._fireEventIfSelectionChanged();
                         }
                         _fireEventIfSelectionChanged() {
                             const _ = this._model.finalSelectionStart,
                                 b = this._model.finalSelectionEnd,
-                                A = !(!_ || !b || _[0] === b[0] && _[1] === b[1]);
-                            A ? _ && b && (this._oldSelectionStart && this._oldSelectionEnd && _[0] === this._oldSelectionStart[0] && _[1] === this._oldSelectionStart[1] && b[0] === this._oldSelectionEnd[0] && b[1] === this._oldSelectionEnd[1] || this._fireOnSelectionChange(_, b, A)) : this._oldHasSelection && this._fireOnSelectionChange(_, b, A);
+                                R = !(!_ || !b || _[0] === b[0] && _[1] === b[1]);
+                            R ? _ && b && (this._oldSelectionStart && this._oldSelectionEnd && _[0] === this._oldSelectionStart[0] && _[1] === this._oldSelectionStart[1] && b[0] === this._oldSelectionEnd[0] && b[1] === this._oldSelectionEnd[1] || this._fireOnSelectionChange(_, b, R)) : this._oldHasSelection && this._fireOnSelectionChange(_, b, R);
                         }
-                        _fireOnSelectionChange(_, b, A) {
-                            this._oldSelectionStart = _, this._oldSelectionEnd = b, this._oldHasSelection = A, this._onSelectionChange.fire();
+                        _fireOnSelectionChange(_, b, R) {
+                            this._oldSelectionStart = _, this._oldSelectionEnd = b, this._oldHasSelection = R, this._onSelectionChange.fire();
                         }
                         _handleBufferActivate(_) {
                             this.clearSelection(), this._trimListener.dispose(), this._trimListener = _.activeBuffer.lines.onTrim((b) => this._handleTrim(b));
                         }
                         _convertViewportColToCharacterIndex(_, b) {
-                            let A = b;
-                            for (let T = 0; b >= T; T++) {
-                                const x = _.loadCell(T, this._workCell).getChars().length;
-                                this._workCell.getWidth() === 0 ? A-- : x > 1 && b !== T && (A += x - 1);
+                            let R = b;
+                            for (let B = 0; b >= B; B++) {
+                                const T = _.loadCell(B, this._workCell).getChars().length;
+                                this._workCell.getWidth() === 0 ? R-- : T > 1 && b !== B && (R += T - 1);
                             }
-                            return A;
+                            return R;
                         }
-                        setSelection(_, b, A) {
-                            this._model.clearSelection(), this._removeMouseDownListeners(), this._model.selectionStart = [_, b], this._model.selectionStartLength = A, this.refresh(), this._fireEventIfSelectionChanged();
+                        setSelection(_, b, R) {
+                            this._model.clearSelection(), this._removeMouseDownListeners(), this._model.selectionStart = [_, b], this._model.selectionStartLength = R, this.refresh(), this._fireEventIfSelectionChanged();
                         }
                         rightClickSelect(_) {
                             this._isClickInSelection(_) || (this._selectWordAtCursor(_, !1) && this.refresh(!0), this._fireEventIfSelectionChanged());
                         }
-                        _getWordAt(_, b, A = !0, T = !0) {
+                        _getWordAt(_, b, R = !0, B = !0) {
                             if (_[0] >= this._bufferService.cols)
                                 return;
-                            const x = this._bufferService.buffer,
-                                L = x.lines.get(_[1]);
+                            const T = this._bufferService.buffer,
+                                L = T.lines.get(_[1]);
                             if (!L)
                                 return;
-                            const H = x.translateBufferLineToString(_[1], !1);
+                            const H = T.translateBufferLineToString(_[1], !1);
                             let W = this._convertViewportColToCharacterIndex(L, _[0]),
-                                U = W;
-                            const K = _[0] - W;
-                            let j = 0,
+                                j = W;
+                            const V = _[0] - W;
+                            let z = 0,
                                 C = 0,
-                                D = 0,
-                                B = 0;
+                                x = 0,
+                                A = 0;
                             if (H.charAt(W) === " ") {
                                 for (; W > 0 && H.charAt(W - 1) === " ";)
                                     W--;
-                                for (; U < H.length && H.charAt(U + 1) === " ";)
-                                    U++;
+                                for (; j < H.length && H.charAt(j + 1) === " ";)
+                                    j++;
                             } else {
-                                let z = _[0],
-                                    G = _[0];
-                                L.getWidth(z) === 0 && (j++, z--), L.getWidth(G) === 2 && (C++, G++);
-                                const X = L.getString(G).length;
-                                for (X > 1 && (B += X - 1, U += X - 1); z > 0 && W > 0 && !this._isCharWordSeparator(L.loadCell(z - 1, this._workCell));) {
-                                    L.loadCell(z - 1, this._workCell);
+                                let q = _[0],
+                                    X = _[0];
+                                L.getWidth(q) === 0 && (z++, q--), L.getWidth(X) === 2 && (C++, X++);
+                                const J = L.getString(X).length;
+                                for (J > 1 && (A += J - 1, j += J - 1); q > 0 && W > 0 && !this._isCharWordSeparator(L.loadCell(q - 1, this._workCell));) {
+                                    L.loadCell(q - 1, this._workCell);
                                     const P = this._workCell.getChars().length;
-                                    this._workCell.getWidth() === 0 ? (j++, z--) : P > 1 && (D += P - 1, W -= P - 1), W--, z--;
+                                    this._workCell.getWidth() === 0 ? (z++, q--) : P > 1 && (x += P - 1, W -= P - 1), W--, q--;
                                 }
-                                for (; G < L.length && U + 1 < H.length && !this._isCharWordSeparator(L.loadCell(G + 1, this._workCell));) {
-                                    L.loadCell(G + 1, this._workCell);
+                                for (; X < L.length && j + 1 < H.length && !this._isCharWordSeparator(L.loadCell(X + 1, this._workCell));) {
+                                    L.loadCell(X + 1, this._workCell);
                                     const P = this._workCell.getChars().length;
-                                    this._workCell.getWidth() === 2 ? (C++, G++) : P > 1 && (B += P - 1, U += P - 1), U++, G++;
+                                    this._workCell.getWidth() === 2 ? (C++, X++) : P > 1 && (A += P - 1, j += P - 1), j++, X++;
                                 }
                             }
-                            U++;
-                            let O = W + K - j + D,
-                                I = Math.min(this._bufferService.cols, U - W + j + C - D - B);
-                            if (b || H.slice(W, U).trim() !== "") {
-                                if (A && O === 0 && L.getCodePoint(0) !== 32) {
-                                    const z = x.lines.get(_[1] - 1);
-                                    if (z && L.isWrapped && z.getCodePoint(this._bufferService.cols - 1) !== 32) {
-                                        const G = this._getWordAt([this._bufferService.cols - 1, _[1] - 1], !1, !0, !1);
-                                        if (G) {
-                                            const X = this._bufferService.cols - G.start;
-                                            O -= X, I += X;
+                            j++;
+                            let O = W + V - z + x,
+                                I = Math.min(this._bufferService.cols, j - W + z + C - x - A);
+                            if (b || H.slice(W, j).trim() !== "") {
+                                if (R && O === 0 && L.getCodePoint(0) !== 32) {
+                                    const q = T.lines.get(_[1] - 1);
+                                    if (q && L.isWrapped && q.getCodePoint(this._bufferService.cols - 1) !== 32) {
+                                        const X = this._getWordAt([this._bufferService.cols - 1, _[1] - 1], !1, !0, !1);
+                                        if (X) {
+                                            const J = this._bufferService.cols - X.start;
+                                            O -= J, I += J;
                                         }
                                     }
                                 }
-                                if (T && O + I === this._bufferService.cols && L.getCodePoint(this._bufferService.cols - 1) !== 32) {
-                                    const z = x.lines.get(_[1] + 1);
-                                    if (z != null && z.isWrapped && z.getCodePoint(0) !== 32) {
-                                        const G = this._getWordAt([0, _[1] + 1], !1, !1, !0);
-                                        G && (I += G.length);
+                                if (B && O + I === this._bufferService.cols && L.getCodePoint(this._bufferService.cols - 1) !== 32) {
+                                    const q = T.lines.get(_[1] + 1);
+                                    if (q != null && q.isWrapped && q.getCodePoint(0) !== 32) {
+                                        const X = this._getWordAt([0, _[1] + 1], !1, !1, !0);
+                                        X && (I += X.length);
                                     }
                                 }
                                 return {
                                     start: O,
                                     length: I
                                 };
                             }
                         }
                         _selectWordAt(_, b) {
-                            const A = this._getWordAt(_, b);
-                            if (A) {
-                                for (; A.start < 0;)
-                                    A.start += this._bufferService.cols, _[1]--;
-                                this._model.selectionStart = [A.start, _[1]], this._model.selectionStartLength = A.length;
+                            const R = this._getWordAt(_, b);
+                            if (R) {
+                                for (; R.start < 0;)
+                                    R.start += this._bufferService.cols, _[1]--;
+                                this._model.selectionStart = [R.start, _[1]], this._model.selectionStartLength = R.length;
                             }
                         }
                         _selectToWordAt(_) {
                             const b = this._getWordAt(_, !0);
                             if (b) {
-                                let A = _[1];
+                                let R = _[1];
                                 for (; b.start < 0;)
-                                    b.start += this._bufferService.cols, A--;
+                                    b.start += this._bufferService.cols, R--;
                                 if (!this._model.areSelectionValuesReversed())
                                     for (; b.start + b.length > this._bufferService.cols;)
-                                        b.length -= this._bufferService.cols, A++;
-                                this._model.selectionEnd = [this._model.areSelectionValuesReversed() ? b.start : b.start + b.length, A];
+                                        b.length -= this._bufferService.cols, R++;
+                                this._model.selectionEnd = [this._model.areSelectionValuesReversed() ? b.start : b.start + b.length, R];
                             }
                         }
                         _isCharWordSeparator(_) {
                             return _.getWidth() !== 0 && this._optionsService.rawOptions.wordSeparator.indexOf(_.getChars()) >= 0;
                         }
                         _selectLineAt(_) {
                             const b = this._bufferService.buffer.getWrappedRangeForLine(_),
-                                A = {
+                                R = {
                                     start: {
                                         x: 0,
                                         y: b.first
                                     },
                                     end: {
                                         x: this._bufferService.cols - 1,
                                         y: b.last
                                     }
                                 };
-                            this._model.selectionStart = [0, b.first], this._model.selectionEnd = void 0, this._model.selectionStartLength = (0, t.getRangeLength)(A, this._bufferService.cols);
+                            this._model.selectionStart = [0, b.first], this._model.selectionEnd = void 0, this._model.selectionStartLength = (0, e.getRangeLength)(R, this._bufferService.cols);
                         }
                     };
-                    i.SelectionService = p = o([c(3, h.IBufferService), c(4, h.ICoreService), c(5, g.IMouseService), c(6, h.IOptionsService), c(7, g.IRenderService), c(8, g.ICoreBrowserService)], p);
+                    i.SelectionService = S = o([c(3, h.IBufferService), c(4, h.ICoreService), c(5, m.IMouseService), c(6, h.IOptionsService), c(7, m.IRenderService), c(8, m.ICoreBrowserService)], S);
                 },
                 4725: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.ILinkProviderService = i.IThemeService = i.ICharacterJoinerService = i.ISelectionService = i.IRenderService = i.IMouseService = i.ICoreBrowserService = i.ICharSizeService = void 0;
                     const o = n(8343);
                     i.ICharSizeService = (0, o.createDecorator)("CharSizeService"), i.ICoreBrowserService = (0, o.createDecorator)("CoreBrowserService"), i.IMouseService = (0, o.createDecorator)("MouseService"), i.IRenderService = (0, o.createDecorator)("RenderService"), i.ISelectionService = (0, o.createDecorator)("SelectionService"), i.ICharacterJoinerService = (0, o.createDecorator)("CharacterJoinerService"), i.IThemeService = (0, o.createDecorator)("ThemeService"), i.ILinkProviderService = (0, o.createDecorator)("LinkProviderService");
                 },
                 6731: function(k, i, n) {
-                    var o = this && this.__decorate || function(p, _, b, A) {
-                            var T, x = arguments.length,
-                                L = x < 3 ? _ : A === null ? A = Object.getOwnPropertyDescriptor(_, b) : A;
+                    var o = this && this.__decorate || function(S, _, b, R) {
+                            var B, T = arguments.length,
+                                L = T < 3 ? _ : R === null ? R = Object.getOwnPropertyDescriptor(_, b) : R;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                L = Reflect.decorate(p, _, b, A);
+                                L = Reflect.decorate(S, _, b, R);
                             else
-                                for (var H = p.length - 1; H >= 0; H--)
-                                    (T = p[H]) && (L = (x < 3 ? T(L) : x > 3 ? T(_, b, L) : T(_, b)) || L);
-                            return x > 3 && L && Object.defineProperty(_, b, L), L;
+                                for (var H = S.length - 1; H >= 0; H--)
+                                    (B = S[H]) && (L = (T < 3 ? B(L) : T > 3 ? B(_, b, L) : B(_, b)) || L);
+                            return T > 3 && L && Object.defineProperty(_, b, L), L;
                         },
-                        c = this && this.__param || function(p, _) {
-                            return function(b, A) {
-                                _(b, A, p);
+                        c = this && this.__param || function(S, _) {
+                            return function(b, R) {
+                                _(b, R, S);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.ThemeService = i.DEFAULT_ANSI_COLORS = void 0;
                     const a = n(7239),
                         d = n(8055),
-                        f = n(8460),
-                        g = n(844),
+                        v = n(8460),
+                        m = n(844),
                         l = n(2585),
                         s = d.css.toColor("#ffffff"),
                         r = d.css.toColor("#000000"),
-                        t = d.css.toColor("#ffffff"),
-                        e = d.css.toColor("#000000"),
+                        e = d.css.toColor("#ffffff"),
+                        t = d.css.toColor("#000000"),
                         h = {
                             css: "rgba(255, 255, 255, 0.3)",
                             rgba: 4294967117
                         };
                     i.DEFAULT_ANSI_COLORS = Object.freeze((() => {
-                        const p = [d.css.toColor("#2e3436"), d.css.toColor("#cc0000"), d.css.toColor("#4e9a06"), d.css.toColor("#c4a000"), d.css.toColor("#3465a4"), d.css.toColor("#75507b"), d.css.toColor("#06989a"), d.css.toColor("#d3d7cf"), d.css.toColor("#555753"), d.css.toColor("#ef2929"), d.css.toColor("#8ae234"), d.css.toColor("#fce94f"), d.css.toColor("#729fcf"), d.css.toColor("#ad7fa8"), d.css.toColor("#34e2e2"), d.css.toColor("#eeeeec")],
+                        const S = [d.css.toColor("#2e3436"), d.css.toColor("#cc0000"), d.css.toColor("#4e9a06"), d.css.toColor("#c4a000"), d.css.toColor("#3465a4"), d.css.toColor("#75507b"), d.css.toColor("#06989a"), d.css.toColor("#d3d7cf"), d.css.toColor("#555753"), d.css.toColor("#ef2929"), d.css.toColor("#8ae234"), d.css.toColor("#fce94f"), d.css.toColor("#729fcf"), d.css.toColor("#ad7fa8"), d.css.toColor("#34e2e2"), d.css.toColor("#eeeeec")],
                             _ = [0, 95, 135, 175, 215, 255];
                         for (let b = 0; b < 216; b++) {
-                            const A = _[b / 36 % 6 | 0],
-                                T = _[b / 6 % 6 | 0],
-                                x = _[b % 6];
-                            p.push({
-                                css: d.channels.toCss(A, T, x),
-                                rgba: d.channels.toRgba(A, T, x)
+                            const R = _[b / 36 % 6 | 0],
+                                B = _[b / 6 % 6 | 0],
+                                T = _[b % 6];
+                            S.push({
+                                css: d.channels.toCss(R, B, T),
+                                rgba: d.channels.toRgba(R, B, T)
                             });
                         }
                         for (let b = 0; b < 24; b++) {
-                            const A = 8 + 10 * b;
-                            p.push({
-                                css: d.channels.toCss(A, A, A),
-                                rgba: d.channels.toRgba(A, A, A)
+                            const R = 8 + 10 * b;
+                            S.push({
+                                css: d.channels.toCss(R, R, R),
+                                rgba: d.channels.toRgba(R, R, R)
                             });
                         }
-                        return p;
+                        return S;
                     })());
-                    let v = i.ThemeService = class extends g.Disposable {
+                    let g = i.ThemeService = class extends m.Disposable {
                         get colors() {
                             return this._colors;
                         }
-                        constructor(p) {
-                            super(), this._optionsService = p, this._contrastCache = new a.ColorContrastCache(), this._halfContrastCache = new a.ColorContrastCache(), this._onChangeColors = this.register(new f.EventEmitter()), this.onChangeColors = this._onChangeColors.event, this._colors = {
+                        constructor(S) {
+                            super(), this._optionsService = S, this._contrastCache = new a.ColorContrastCache(), this._halfContrastCache = new a.ColorContrastCache(), this._onChangeColors = this.register(new v.EventEmitter()), this.onChangeColors = this._onChangeColors.event, this._colors = {
                                 foreground: s,
                                 background: r,
-                                cursor: t,
-                                cursorAccent: e,
+                                cursor: e,
+                                cursorAccent: t,
                                 selectionForeground: void 0,
                                 selectionBackgroundTransparent: h,
                                 selectionBackgroundOpaque: d.color.blend(r, h),
                                 selectionInactiveBackgroundTransparent: h,
                                 selectionInactiveBackgroundOpaque: d.color.blend(r, h),
                                 ansi: i.DEFAULT_ANSI_COLORS.slice(),
                                 contrastCache: this._contrastCache,
                                 halfContrastCache: this._halfContrastCache
                             }, this._updateRestoreColors(), this._setTheme(this._optionsService.rawOptions.theme), this.register(this._optionsService.onSpecificOptionChange("minimumContrastRatio", () => this._contrastCache.clear())), this.register(this._optionsService.onSpecificOptionChange("theme", () => this._setTheme(this._optionsService.rawOptions.theme)));
                         }
-                        _setTheme(p = {}) {
+                        _setTheme(S = {}) {
                             const _ = this._colors;
-                            if (_.foreground = u(p.foreground, s), _.background = u(p.background, r), _.cursor = u(p.cursor, t), _.cursorAccent = u(p.cursorAccent, e), _.selectionBackgroundTransparent = u(p.selectionBackground, h), _.selectionBackgroundOpaque = d.color.blend(_.background, _.selectionBackgroundTransparent), _.selectionInactiveBackgroundTransparent = u(p.selectionInactiveBackground, _.selectionBackgroundTransparent), _.selectionInactiveBackgroundOpaque = d.color.blend(_.background, _.selectionInactiveBackgroundTransparent), _.selectionForeground = p.selectionForeground ? u(p.selectionForeground, d.NULL_COLOR) : void 0, _.selectionForeground === d.NULL_COLOR && (_.selectionForeground = void 0), d.color.isOpaque(_.selectionBackgroundTransparent) && (_.selectionBackgroundTransparent = d.color.opacity(_.selectionBackgroundTransparent, 0.3)), d.color.isOpaque(_.selectionInactiveBackgroundTransparent) && (_.selectionInactiveBackgroundTransparent = d.color.opacity(_.selectionInactiveBackgroundTransparent, 0.3)), _.ansi = i.DEFAULT_ANSI_COLORS.slice(), _.ansi[0] = u(p.black, i.DEFAULT_ANSI_COLORS[0]), _.ansi[1] = u(p.red, i.DEFAULT_ANSI_COLORS[1]), _.ansi[2] = u(p.green, i.DEFAULT_ANSI_COLORS[2]), _.ansi[3] = u(p.yellow, i.DEFAULT_ANSI_COLORS[3]), _.ansi[4] = u(p.blue, i.DEFAULT_ANSI_COLORS[4]), _.ansi[5] = u(p.magenta, i.DEFAULT_ANSI_COLORS[5]), _.ansi[6] = u(p.cyan, i.DEFAULT_ANSI_COLORS[6]), _.ansi[7] = u(p.white, i.DEFAULT_ANSI_COLORS[7]), _.ansi[8] = u(p.brightBlack, i.DEFAULT_ANSI_COLORS[8]), _.ansi[9] = u(p.brightRed, i.DEFAULT_ANSI_COLORS[9]), _.ansi[10] = u(p.brightGreen, i.DEFAULT_ANSI_COLORS[10]), _.ansi[11] = u(p.brightYellow, i.DEFAULT_ANSI_COLORS[11]), _.ansi[12] = u(p.brightBlue, i.DEFAULT_ANSI_COLORS[12]), _.ansi[13] = u(p.brightMagenta, i.DEFAULT_ANSI_COLORS[13]), _.ansi[14] = u(p.brightCyan, i.DEFAULT_ANSI_COLORS[14]), _.ansi[15] = u(p.brightWhite, i.DEFAULT_ANSI_COLORS[15]), p.extendedAnsi) {
-                                const b = Math.min(_.ansi.length - 16, p.extendedAnsi.length);
-                                for (let A = 0; A < b; A++)
-                                    _.ansi[A + 16] = u(p.extendedAnsi[A], i.DEFAULT_ANSI_COLORS[A + 16]);
+                            if (_.foreground = u(S.foreground, s), _.background = u(S.background, r), _.cursor = u(S.cursor, e), _.cursorAccent = u(S.cursorAccent, t), _.selectionBackgroundTransparent = u(S.selectionBackground, h), _.selectionBackgroundOpaque = d.color.blend(_.background, _.selectionBackgroundTransparent), _.selectionInactiveBackgroundTransparent = u(S.selectionInactiveBackground, _.selectionBackgroundTransparent), _.selectionInactiveBackgroundOpaque = d.color.blend(_.background, _.selectionInactiveBackgroundTransparent), _.selectionForeground = S.selectionForeground ? u(S.selectionForeground, d.NULL_COLOR) : void 0, _.selectionForeground === d.NULL_COLOR && (_.selectionForeground = void 0), d.color.isOpaque(_.selectionBackgroundTransparent) && (_.selectionBackgroundTransparent = d.color.opacity(_.selectionBackgroundTransparent, 0.3)), d.color.isOpaque(_.selectionInactiveBackgroundTransparent) && (_.selectionInactiveBackgroundTransparent = d.color.opacity(_.selectionInactiveBackgroundTransparent, 0.3)), _.ansi = i.DEFAULT_ANSI_COLORS.slice(), _.ansi[0] = u(S.black, i.DEFAULT_ANSI_COLORS[0]), _.ansi[1] = u(S.red, i.DEFAULT_ANSI_COLORS[1]), _.ansi[2] = u(S.green, i.DEFAULT_ANSI_COLORS[2]), _.ansi[3] = u(S.yellow, i.DEFAULT_ANSI_COLORS[3]), _.ansi[4] = u(S.blue, i.DEFAULT_ANSI_COLORS[4]), _.ansi[5] = u(S.magenta, i.DEFAULT_ANSI_COLORS[5]), _.ansi[6] = u(S.cyan, i.DEFAULT_ANSI_COLORS[6]), _.ansi[7] = u(S.white, i.DEFAULT_ANSI_COLORS[7]), _.ansi[8] = u(S.brightBlack, i.DEFAULT_ANSI_COLORS[8]), _.ansi[9] = u(S.brightRed, i.DEFAULT_ANSI_COLORS[9]), _.ansi[10] = u(S.brightGreen, i.DEFAULT_ANSI_COLORS[10]), _.ansi[11] = u(S.brightYellow, i.DEFAULT_ANSI_COLORS[11]), _.ansi[12] = u(S.brightBlue, i.DEFAULT_ANSI_COLORS[12]), _.ansi[13] = u(S.brightMagenta, i.DEFAULT_ANSI_COLORS[13]), _.ansi[14] = u(S.brightCyan, i.DEFAULT_ANSI_COLORS[14]), _.ansi[15] = u(S.brightWhite, i.DEFAULT_ANSI_COLORS[15]), S.extendedAnsi) {
+                                const b = Math.min(_.ansi.length - 16, S.extendedAnsi.length);
+                                for (let R = 0; R < b; R++)
+                                    _.ansi[R + 16] = u(S.extendedAnsi[R], i.DEFAULT_ANSI_COLORS[R + 16]);
                             }
                             this._contrastCache.clear(), this._halfContrastCache.clear(), this._updateRestoreColors(), this._onChangeColors.fire(this.colors);
                         }
-                        restoreColor(p) {
-                            this._restoreColor(p), this._onChangeColors.fire(this.colors);
+                        restoreColor(S) {
+                            this._restoreColor(S), this._onChangeColors.fire(this.colors);
                         }
-                        _restoreColor(p) {
-                            if (p !== void 0)
-                                switch (p) {
+                        _restoreColor(S) {
+                            if (S !== void 0)
+                                switch (S) {
                                     case 256:
                                         this._colors.foreground = this._restoreColors.foreground;
                                         break;
                                     case 257:
                                         this._colors.background = this._restoreColors.background;
                                         break;
                                     case 258:
                                         this._colors.cursor = this._restoreColors.cursor;
                                         break;
                                     default:
-                                        this._colors.ansi[p] = this._restoreColors.ansi[p];
+                                        this._colors.ansi[S] = this._restoreColors.ansi[S];
                                 }
                             else
                                 for (let _ = 0; _ < this._restoreColors.ansi.length; ++_)
                                     this._colors.ansi[_] = this._restoreColors.ansi[_];
                         }
-                        modifyColors(p) {
-                            p(this._colors), this._onChangeColors.fire(this.colors);
+                        modifyColors(S) {
+                            S(this._colors), this._onChangeColors.fire(this.colors);
                         }
                         _updateRestoreColors() {
                             this._restoreColors = {
                                 foreground: this._colors.foreground,
                                 background: this._colors.background,
                                 cursor: this._colors.cursor,
                                 ansi: this._colors.ansi.slice()
                             };
                         }
                     };
 
-                    function u(p, _) {
-                        if (p !== void 0)
+                    function u(S, _) {
+                        if (S !== void 0)
                             try {
-                                return d.css.toColor(p);
+                                return d.css.toColor(S);
                             } catch {}
                         return _;
                     }
-                    i.ThemeService = v = o([c(0, l.IOptionsService)], v);
+                    i.ThemeService = g = o([c(0, l.IOptionsService)], g);
                 },
                 6349: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CircularList = void 0;
                     const o = n(8460),
                         c = n(844);
                     class a extends c.Disposable {
-                        constructor(f) {
-                            super(), this._maxLength = f, this.onDeleteEmitter = this.register(new o.EventEmitter()), this.onDelete = this.onDeleteEmitter.event, this.onInsertEmitter = this.register(new o.EventEmitter()), this.onInsert = this.onInsertEmitter.event, this.onTrimEmitter = this.register(new o.EventEmitter()), this.onTrim = this.onTrimEmitter.event, this._array = new Array(this._maxLength), this._startIndex = 0, this._length = 0;
+                        constructor(v) {
+                            super(), this._maxLength = v, this.onDeleteEmitter = this.register(new o.EventEmitter()), this.onDelete = this.onDeleteEmitter.event, this.onInsertEmitter = this.register(new o.EventEmitter()), this.onInsert = this.onInsertEmitter.event, this.onTrimEmitter = this.register(new o.EventEmitter()), this.onTrim = this.onTrimEmitter.event, this._array = new Array(this._maxLength), this._startIndex = 0, this._length = 0;
                         }
                         get maxLength() {
                             return this._maxLength;
                         }
-                        set maxLength(f) {
-                            if (this._maxLength === f)
+                        set maxLength(v) {
+                            if (this._maxLength === v)
                                 return;
-                            const g = new Array(f);
-                            for (let l = 0; l < Math.min(f, this.length); l++)
-                                g[l] = this._array[this._getCyclicIndex(l)];
-                            this._array = g, this._maxLength = f, this._startIndex = 0;
+                            const m = new Array(v);
+                            for (let l = 0; l < Math.min(v, this.length); l++)
+                                m[l] = this._array[this._getCyclicIndex(l)];
+                            this._array = m, this._maxLength = v, this._startIndex = 0;
                         }
                         get length() {
                             return this._length;
                         }
-                        set length(f) {
-                            if (f > this._length)
-                                for (let g = this._length; g < f; g++)
-                                    this._array[g] = void 0;
-                            this._length = f;
+                        set length(v) {
+                            if (v > this._length)
+                                for (let m = this._length; m < v; m++)
+                                    this._array[m] = void 0;
+                            this._length = v;
                         }
-                        get(f) {
-                            return this._array[this._getCyclicIndex(f)];
+                        get(v) {
+                            return this._array[this._getCyclicIndex(v)];
                         }
-                        set(f, g) {
-                            this._array[this._getCyclicIndex(f)] = g;
+                        set(v, m) {
+                            this._array[this._getCyclicIndex(v)] = m;
                         }
-                        push(f) {
-                            this._array[this._getCyclicIndex(this._length)] = f, this._length === this._maxLength ? (this._startIndex = ++this._startIndex % this._maxLength, this.onTrimEmitter.fire(1)) : this._length++;
+                        push(v) {
+                            this._array[this._getCyclicIndex(this._length)] = v, this._length === this._maxLength ? (this._startIndex = ++this._startIndex % this._maxLength, this.onTrimEmitter.fire(1)) : this._length++;
                         }
                         recycle() {
                             if (this._length !== this._maxLength)
                                 throw new Error("Can only recycle when the buffer is full");
                             return this._startIndex = ++this._startIndex % this._maxLength, this.onTrimEmitter.fire(1), this._array[this._getCyclicIndex(this._length - 1)];
                         }
                         get isFull() {
                             return this._length === this._maxLength;
                         }
                         pop() {
                             return this._array[this._getCyclicIndex(this._length-- - 1)];
                         }
-                        splice(f, g, ...l) {
-                            if (g) {
-                                for (let s = f; s < this._length - g; s++)
-                                    this._array[this._getCyclicIndex(s)] = this._array[this._getCyclicIndex(s + g)];
-                                this._length -= g, this.onDeleteEmitter.fire({
-                                    index: f,
-                                    amount: g
+                        splice(v, m, ...l) {
+                            if (m) {
+                                for (let s = v; s < this._length - m; s++)
+                                    this._array[this._getCyclicIndex(s)] = this._array[this._getCyclicIndex(s + m)];
+                                this._length -= m, this.onDeleteEmitter.fire({
+                                    index: v,
+                                    amount: m
                                 });
                             }
-                            for (let s = this._length - 1; s >= f; s--)
+                            for (let s = this._length - 1; s >= v; s--)
                                 this._array[this._getCyclicIndex(s + l.length)] = this._array[this._getCyclicIndex(s)];
                             for (let s = 0; s < l.length; s++)
-                                this._array[this._getCyclicIndex(f + s)] = l[s];
+                                this._array[this._getCyclicIndex(v + s)] = l[s];
                             if (l.length && this.onInsertEmitter.fire({
-                                    index: f,
+                                    index: v,
                                     amount: l.length
                                 }), this._length + l.length > this._maxLength) {
                                 const s = this._length + l.length - this._maxLength;
                                 this._startIndex += s, this._length = this._maxLength, this.onTrimEmitter.fire(s);
                             } else
                                 this._length += l.length;
                         }
-                        trimStart(f) {
-                            f > this._length && (f = this._length), this._startIndex += f, this._length -= f, this.onTrimEmitter.fire(f);
+                        trimStart(v) {
+                            v > this._length && (v = this._length), this._startIndex += v, this._length -= v, this.onTrimEmitter.fire(v);
                         }
-                        shiftElements(f, g, l) {
-                            if (!(g <= 0)) {
-                                if (f < 0 || f >= this._length)
+                        shiftElements(v, m, l) {
+                            if (!(m <= 0)) {
+                                if (v < 0 || v >= this._length)
                                     throw new Error("start argument out of range");
-                                if (f + l < 0)
+                                if (v + l < 0)
                                     throw new Error("Cannot shift elements in list beyond index 0");
                                 if (l > 0) {
-                                    for (let r = g - 1; r >= 0; r--)
-                                        this.set(f + r + l, this.get(f + r));
-                                    const s = f + g + l - this._length;
+                                    for (let r = m - 1; r >= 0; r--)
+                                        this.set(v + r + l, this.get(v + r));
+                                    const s = v + m + l - this._length;
                                     if (s > 0)
                                         for (this._length += s; this._length > this._maxLength;)
                                             this._length--, this._startIndex++, this.onTrimEmitter.fire(1);
                                 } else
-                                    for (let s = 0; s < g; s++)
-                                        this.set(f + s + l, this.get(f + s));
+                                    for (let s = 0; s < m; s++)
+                                        this.set(v + s + l, this.get(v + s));
                             }
                         }
-                        _getCyclicIndex(f) {
-                            return (this._startIndex + f) % this._maxLength;
+                        _getCyclicIndex(v) {
+                            return (this._startIndex + v) % this._maxLength;
                         }
                     }
                     i.CircularList = a;
                 },
                 1439: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
@@ -5537,92 +5537,92 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.contrastRatio = i.toPaddedHex = i.rgba = i.rgb = i.css = i.color = i.channels = i.NULL_COLOR = void 0;
                     let n = 0,
                         o = 0,
                         c = 0,
                         a = 0;
-                    var d, f, g, l, s;
+                    var d, v, m, l, s;
 
-                    function r(e) {
-                        const h = e.toString(16);
+                    function r(t) {
+                        const h = t.toString(16);
                         return h.length < 2 ? "0" + h : h;
                     }
 
-                    function t(e, h) {
-                        return e < h ? (h + 0.05) / (e + 0.05) : (e + 0.05) / (h + 0.05);
+                    function e(t, h) {
+                        return t < h ? (h + 0.05) / (t + 0.05) : (t + 0.05) / (h + 0.05);
                     }
                     i.NULL_COLOR = {
                             css: "#00000000",
                             rgba: 0
                         },
-                        function(e) {
-                            e.toCss = function(h, v, u, p) {
-                                return p !== void 0 ? `#${r(h)}${r(v)}${r(u)}${r(p)}` : `#${r(h)}${r(v)}${r(u)}`;
-                            }, e.toRgba = function(h, v, u, p = 255) {
-                                return (h << 24 | v << 16 | u << 8 | p) >>> 0;
-                            }, e.toColor = function(h, v, u, p) {
+                        function(t) {
+                            t.toCss = function(h, g, u, S) {
+                                return S !== void 0 ? `#${r(h)}${r(g)}${r(u)}${r(S)}` : `#${r(h)}${r(g)}${r(u)}`;
+                            }, t.toRgba = function(h, g, u, S = 255) {
+                                return (h << 24 | g << 16 | u << 8 | S) >>> 0;
+                            }, t.toColor = function(h, g, u, S) {
                                 return {
-                                    css: e.toCss(h, v, u, p),
-                                    rgba: e.toRgba(h, v, u, p)
+                                    css: t.toCss(h, g, u, S),
+                                    rgba: t.toRgba(h, g, u, S)
                                 };
                             };
                         }(d || (i.channels = d = {})),
-                        function(e) {
-                            function h(v, u) {
-                                return a = Math.round(255 * u), [n, o, c] = s.toChannels(v.rgba), {
+                        function(t) {
+                            function h(g, u) {
+                                return a = Math.round(255 * u), [n, o, c] = s.toChannels(g.rgba), {
                                     css: d.toCss(n, o, c, a),
                                     rgba: d.toRgba(n, o, c, a)
                                 };
                             }
-                            e.blend = function(v, u) {
+                            t.blend = function(g, u) {
                                 if (a = (255 & u.rgba) / 255, a === 1)
                                     return {
                                         css: u.css,
                                         rgba: u.rgba
                                     };
-                                const p = u.rgba >> 24 & 255,
+                                const S = u.rgba >> 24 & 255,
                                     _ = u.rgba >> 16 & 255,
                                     b = u.rgba >> 8 & 255,
-                                    A = v.rgba >> 24 & 255,
-                                    T = v.rgba >> 16 & 255,
-                                    x = v.rgba >> 8 & 255;
-                                return n = A + Math.round((p - A) * a), o = T + Math.round((_ - T) * a), c = x + Math.round((b - x) * a), {
+                                    R = g.rgba >> 24 & 255,
+                                    B = g.rgba >> 16 & 255,
+                                    T = g.rgba >> 8 & 255;
+                                return n = R + Math.round((S - R) * a), o = B + Math.round((_ - B) * a), c = T + Math.round((b - T) * a), {
                                     css: d.toCss(n, o, c),
                                     rgba: d.toRgba(n, o, c)
                                 };
-                            }, e.isOpaque = function(v) {
-                                return (255 & v.rgba) == 255;
-                            }, e.ensureContrastRatio = function(v, u, p) {
-                                const _ = s.ensureContrastRatio(v.rgba, u.rgba, p);
+                            }, t.isOpaque = function(g) {
+                                return (255 & g.rgba) == 255;
+                            }, t.ensureContrastRatio = function(g, u, S) {
+                                const _ = s.ensureContrastRatio(g.rgba, u.rgba, S);
                                 if (_)
                                     return d.toColor(_ >> 24 & 255, _ >> 16 & 255, _ >> 8 & 255);
-                            }, e.opaque = function(v) {
-                                const u = (255 | v.rgba) >>> 0;
+                            }, t.opaque = function(g) {
+                                const u = (255 | g.rgba) >>> 0;
                                 return [n, o, c] = s.toChannels(u), {
                                     css: d.toCss(n, o, c),
                                     rgba: u
                                 };
-                            }, e.opacity = h, e.multiplyOpacity = function(v, u) {
-                                return a = 255 & v.rgba, h(v, a * u / 255);
-                            }, e.toColorRGB = function(v) {
-                                return [v.rgba >> 24 & 255, v.rgba >> 16 & 255, v.rgba >> 8 & 255];
-                            };
-                        }(f || (i.color = f = {})),
-                        function(e) {
-                            let h, v;
+                            }, t.opacity = h, t.multiplyOpacity = function(g, u) {
+                                return a = 255 & g.rgba, h(g, a * u / 255);
+                            }, t.toColorRGB = function(g) {
+                                return [g.rgba >> 24 & 255, g.rgba >> 16 & 255, g.rgba >> 8 & 255];
+                            };
+                        }(v || (i.color = v = {})),
+                        function(t) {
+                            let h, g;
                             try {
                                 const u = document.createElement("canvas");
                                 u.width = 1, u.height = 1;
-                                const p = u.getContext("2d", {
+                                const S = u.getContext("2d", {
                                     willReadFrequently: !0
                                 });
-                                p && (h = p, h.globalCompositeOperation = "copy", v = h.createLinearGradient(0, 0, 1, 1));
+                                S && (h = S, h.globalCompositeOperation = "copy", g = h.createLinearGradient(0, 0, 1, 1));
                             } catch {}
-                            e.toColor = function(u) {
+                            t.toColor = function(u) {
                                 if (u.match(/#[\da-f]{3,8}/i))
                                     switch (u.length) {
                                         case 4:
                                             return n = parseInt(u.slice(1, 2).repeat(2), 16), o = parseInt(u.slice(2, 3).repeat(2), 16), c = parseInt(u.slice(3, 4).repeat(2), 16), d.toColor(n, o, c);
                                         case 5:
                                             return n = parseInt(u.slice(1, 2).repeat(2), 16), o = parseInt(u.slice(2, 3).repeat(2), 16), c = parseInt(u.slice(3, 4).repeat(2), 16), a = parseInt(u.slice(4, 5).repeat(2), 16), d.toColor(n, o, c, a);
                                         case 7:
@@ -5630,220 +5630,220 @@
                                                 css: u, rgba: (parseInt(u.slice(1), 16) << 8 | 255) >>> 0
                                             };
                                         case 9:
                                             return {
                                                 css: u, rgba: parseInt(u.slice(1), 16) >>> 0
                                             };
                                     }
-                                const p = u.match(/rgba?\(\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(\d{1,3})\s*(,\s*(0|1|\d?\.(\d+))\s*)?\)/);
-                                if (p)
-                                    return n = parseInt(p[1]), o = parseInt(p[2]), c = parseInt(p[3]), a = Math.round(255 * (p[5] === void 0 ? 1 : parseFloat(p[5]))), d.toColor(n, o, c, a);
-                                if (!h || !v)
+                                const S = u.match(/rgba?\(\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(\d{1,3})\s*(,\s*(0|1|\d?\.(\d+))\s*)?\)/);
+                                if (S)
+                                    return n = parseInt(S[1]), o = parseInt(S[2]), c = parseInt(S[3]), a = Math.round(255 * (S[5] === void 0 ? 1 : parseFloat(S[5]))), d.toColor(n, o, c, a);
+                                if (!h || !g)
                                     throw new Error("css.toColor: Unsupported css format");
-                                if (h.fillStyle = v, h.fillStyle = u, typeof h.fillStyle != "string")
+                                if (h.fillStyle = g, h.fillStyle = u, typeof h.fillStyle != "string")
                                     throw new Error("css.toColor: Unsupported css format");
                                 if (h.fillRect(0, 0, 1, 1), [n, o, c, a] = h.getImageData(0, 0, 1, 1).data, a !== 255)
                                     throw new Error("css.toColor: Unsupported css format");
                                 return {
                                     rgba: d.toRgba(n, o, c, a),
                                     css: u
                                 };
                             };
-                        }(g || (i.css = g = {})),
-                        function(e) {
-                            function h(v, u, p) {
-                                const _ = v / 255,
+                        }(m || (i.css = m = {})),
+                        function(t) {
+                            function h(g, u, S) {
+                                const _ = g / 255,
                                     b = u / 255,
-                                    A = p / 255;
-                                return 0.2126 * (_ <= 0.03928 ? _ / 12.92 : Math.pow((_ + 0.055) / 1.055, 2.4)) + 0.7152 * (b <= 0.03928 ? b / 12.92 : Math.pow((b + 0.055) / 1.055, 2.4)) + 0.0722 * (A <= 0.03928 ? A / 12.92 : Math.pow((A + 0.055) / 1.055, 2.4));
+                                    R = S / 255;
+                                return 0.2126 * (_ <= 0.03928 ? _ / 12.92 : Math.pow((_ + 0.055) / 1.055, 2.4)) + 0.7152 * (b <= 0.03928 ? b / 12.92 : Math.pow((b + 0.055) / 1.055, 2.4)) + 0.0722 * (R <= 0.03928 ? R / 12.92 : Math.pow((R + 0.055) / 1.055, 2.4));
                             }
-                            e.relativeLuminance = function(v) {
-                                return h(v >> 16 & 255, v >> 8 & 255, 255 & v);
-                            }, e.relativeLuminance2 = h;
+                            t.relativeLuminance = function(g) {
+                                return h(g >> 16 & 255, g >> 8 & 255, 255 & g);
+                            }, t.relativeLuminance2 = h;
                         }(l || (i.rgb = l = {})),
-                        function(e) {
-                            function h(u, p, _) {
+                        function(t) {
+                            function h(u, S, _) {
                                 const b = u >> 24 & 255,
-                                    A = u >> 16 & 255,
-                                    T = u >> 8 & 255;
-                                let x = p >> 24 & 255,
-                                    L = p >> 16 & 255,
-                                    H = p >> 8 & 255,
-                                    W = t(l.relativeLuminance2(x, L, H), l.relativeLuminance2(b, A, T));
-                                for (; W < _ && (x > 0 || L > 0 || H > 0);)
-                                    x -= Math.max(0, Math.ceil(0.1 * x)), L -= Math.max(0, Math.ceil(0.1 * L)), H -= Math.max(0, Math.ceil(0.1 * H)), W = t(l.relativeLuminance2(x, L, H), l.relativeLuminance2(b, A, T));
-                                return (x << 24 | L << 16 | H << 8 | 255) >>> 0;
+                                    R = u >> 16 & 255,
+                                    B = u >> 8 & 255;
+                                let T = S >> 24 & 255,
+                                    L = S >> 16 & 255,
+                                    H = S >> 8 & 255,
+                                    W = e(l.relativeLuminance2(T, L, H), l.relativeLuminance2(b, R, B));
+                                for (; W < _ && (T > 0 || L > 0 || H > 0);)
+                                    T -= Math.max(0, Math.ceil(0.1 * T)), L -= Math.max(0, Math.ceil(0.1 * L)), H -= Math.max(0, Math.ceil(0.1 * H)), W = e(l.relativeLuminance2(T, L, H), l.relativeLuminance2(b, R, B));
+                                return (T << 24 | L << 16 | H << 8 | 255) >>> 0;
                             }
 
-                            function v(u, p, _) {
+                            function g(u, S, _) {
                                 const b = u >> 24 & 255,
-                                    A = u >> 16 & 255,
-                                    T = u >> 8 & 255;
-                                let x = p >> 24 & 255,
-                                    L = p >> 16 & 255,
-                                    H = p >> 8 & 255,
-                                    W = t(l.relativeLuminance2(x, L, H), l.relativeLuminance2(b, A, T));
-                                for (; W < _ && (x < 255 || L < 255 || H < 255);)
-                                    x = Math.min(255, x + Math.ceil(0.1 * (255 - x))), L = Math.min(255, L + Math.ceil(0.1 * (255 - L))), H = Math.min(255, H + Math.ceil(0.1 * (255 - H))), W = t(l.relativeLuminance2(x, L, H), l.relativeLuminance2(b, A, T));
-                                return (x << 24 | L << 16 | H << 8 | 255) >>> 0;
-                            }
-                            e.blend = function(u, p) {
-                                if (a = (255 & p) / 255, a === 1)
-                                    return p;
-                                const _ = p >> 24 & 255,
-                                    b = p >> 16 & 255,
-                                    A = p >> 8 & 255,
-                                    T = u >> 24 & 255,
-                                    x = u >> 16 & 255,
+                                    R = u >> 16 & 255,
+                                    B = u >> 8 & 255;
+                                let T = S >> 24 & 255,
+                                    L = S >> 16 & 255,
+                                    H = S >> 8 & 255,
+                                    W = e(l.relativeLuminance2(T, L, H), l.relativeLuminance2(b, R, B));
+                                for (; W < _ && (T < 255 || L < 255 || H < 255);)
+                                    T = Math.min(255, T + Math.ceil(0.1 * (255 - T))), L = Math.min(255, L + Math.ceil(0.1 * (255 - L))), H = Math.min(255, H + Math.ceil(0.1 * (255 - H))), W = e(l.relativeLuminance2(T, L, H), l.relativeLuminance2(b, R, B));
+                                return (T << 24 | L << 16 | H << 8 | 255) >>> 0;
+                            }
+                            t.blend = function(u, S) {
+                                if (a = (255 & S) / 255, a === 1)
+                                    return S;
+                                const _ = S >> 24 & 255,
+                                    b = S >> 16 & 255,
+                                    R = S >> 8 & 255,
+                                    B = u >> 24 & 255,
+                                    T = u >> 16 & 255,
                                     L = u >> 8 & 255;
-                                return n = T + Math.round((_ - T) * a), o = x + Math.round((b - x) * a), c = L + Math.round((A - L) * a), d.toRgba(n, o, c);
-                            }, e.ensureContrastRatio = function(u, p, _) {
+                                return n = B + Math.round((_ - B) * a), o = T + Math.round((b - T) * a), c = L + Math.round((R - L) * a), d.toRgba(n, o, c);
+                            }, t.ensureContrastRatio = function(u, S, _) {
                                 const b = l.relativeLuminance(u >> 8),
-                                    A = l.relativeLuminance(p >> 8);
-                                if (t(b, A) < _) {
-                                    if (A < b) {
-                                        const L = h(u, p, _),
-                                            H = t(b, l.relativeLuminance(L >> 8));
+                                    R = l.relativeLuminance(S >> 8);
+                                if (e(b, R) < _) {
+                                    if (R < b) {
+                                        const L = h(u, S, _),
+                                            H = e(b, l.relativeLuminance(L >> 8));
                                         if (H < _) {
-                                            const W = v(u, p, _);
-                                            return H > t(b, l.relativeLuminance(W >> 8)) ? L : W;
+                                            const W = g(u, S, _);
+                                            return H > e(b, l.relativeLuminance(W >> 8)) ? L : W;
                                         }
                                         return L;
                                     }
-                                    const T = v(u, p, _),
-                                        x = t(b, l.relativeLuminance(T >> 8));
-                                    if (x < _) {
-                                        const L = h(u, p, _);
-                                        return x > t(b, l.relativeLuminance(L >> 8)) ? T : L;
+                                    const B = g(u, S, _),
+                                        T = e(b, l.relativeLuminance(B >> 8));
+                                    if (T < _) {
+                                        const L = h(u, S, _);
+                                        return T > e(b, l.relativeLuminance(L >> 8)) ? B : L;
                                     }
-                                    return T;
+                                    return B;
                                 }
-                            }, e.reduceLuminance = h, e.increaseLuminance = v, e.toChannels = function(u) {
+                            }, t.reduceLuminance = h, t.increaseLuminance = g, t.toChannels = function(u) {
                                 return [u >> 24 & 255, u >> 16 & 255, u >> 8 & 255, 255 & u];
                             };
-                        }(s || (i.rgba = s = {})), i.toPaddedHex = r, i.contrastRatio = t;
+                        }(s || (i.rgba = s = {})), i.toPaddedHex = r, i.contrastRatio = e;
                 },
                 8969: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CoreTerminal = void 0;
                     const o = n(844),
                         c = n(2585),
                         a = n(4348),
                         d = n(7866),
-                        f = n(744),
-                        g = n(7302),
+                        v = n(744),
+                        m = n(7302),
                         l = n(6975),
                         s = n(8460),
                         r = n(1753),
-                        t = n(1480),
-                        e = n(7994),
+                        e = n(1480),
+                        t = n(7994),
                         h = n(9282),
-                        v = n(5435),
+                        g = n(5435),
                         u = n(5981),
-                        p = n(2660);
+                        S = n(2660);
                     let _ = !1;
                     class b extends o.Disposable {
                         get onScroll() {
-                            return this._onScrollApi || (this._onScrollApi = this.register(new s.EventEmitter()), this._onScroll.event((T) => {
-                                var x;
-                                (x = this._onScrollApi) == null || x.fire(T.position);
+                            return this._onScrollApi || (this._onScrollApi = this.register(new s.EventEmitter()), this._onScroll.event((B) => {
+                                var T;
+                                (T = this._onScrollApi) == null || T.fire(B.position);
                             })), this._onScrollApi.event;
                         }
                         get cols() {
                             return this._bufferService.cols;
                         }
                         get rows() {
                             return this._bufferService.rows;
                         }
                         get buffers() {
                             return this._bufferService.buffers;
                         }
                         get options() {
                             return this.optionsService.options;
                         }
-                        set options(T) {
-                            for (const x in T)
-                                this.optionsService.options[x] = T[x];
+                        set options(B) {
+                            for (const T in B)
+                                this.optionsService.options[T] = B[T];
                         }
-                        constructor(T) {
-                            super(), this._windowsWrappingHeuristics = this.register(new o.MutableDisposable()), this._onBinary = this.register(new s.EventEmitter()), this.onBinary = this._onBinary.event, this._onData = this.register(new s.EventEmitter()), this.onData = this._onData.event, this._onLineFeed = this.register(new s.EventEmitter()), this.onLineFeed = this._onLineFeed.event, this._onResize = this.register(new s.EventEmitter()), this.onResize = this._onResize.event, this._onWriteParsed = this.register(new s.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event, this._onScroll = this.register(new s.EventEmitter()), this._instantiationService = new a.InstantiationService(), this.optionsService = this.register(new g.OptionsService(T)), this._instantiationService.setService(c.IOptionsService, this.optionsService), this._bufferService = this.register(this._instantiationService.createInstance(f.BufferService)), this._instantiationService.setService(c.IBufferService, this._bufferService), this._logService = this.register(this._instantiationService.createInstance(d.LogService)), this._instantiationService.setService(c.ILogService, this._logService), this.coreService = this.register(this._instantiationService.createInstance(l.CoreService)), this._instantiationService.setService(c.ICoreService, this.coreService), this.coreMouseService = this.register(this._instantiationService.createInstance(r.CoreMouseService)), this._instantiationService.setService(c.ICoreMouseService, this.coreMouseService), this.unicodeService = this.register(this._instantiationService.createInstance(t.UnicodeService)), this._instantiationService.setService(c.IUnicodeService, this.unicodeService), this._charsetService = this._instantiationService.createInstance(e.CharsetService), this._instantiationService.setService(c.ICharsetService, this._charsetService), this._oscLinkService = this._instantiationService.createInstance(p.OscLinkService), this._instantiationService.setService(c.IOscLinkService, this._oscLinkService), this._inputHandler = this.register(new v.InputHandler(this._bufferService, this._charsetService, this.coreService, this._logService, this.optionsService, this._oscLinkService, this.coreMouseService, this.unicodeService)), this.register((0, s.forwardEvent)(this._inputHandler.onLineFeed, this._onLineFeed)), this.register(this._inputHandler), this.register((0, s.forwardEvent)(this._bufferService.onResize, this._onResize)), this.register((0, s.forwardEvent)(this.coreService.onData, this._onData)), this.register((0, s.forwardEvent)(this.coreService.onBinary, this._onBinary)), this.register(this.coreService.onRequestScrollToBottom(() => this.scrollToBottom())), this.register(this.coreService.onUserInput(() => this._writeBuffer.handleUserInput())), this.register(this.optionsService.onMultipleOptionChange(["windowsMode", "windowsPty"], () => this._handleWindowsPtyOptionChange())), this.register(this._bufferService.onScroll((x) => {
+                        constructor(B) {
+                            super(), this._windowsWrappingHeuristics = this.register(new o.MutableDisposable()), this._onBinary = this.register(new s.EventEmitter()), this.onBinary = this._onBinary.event, this._onData = this.register(new s.EventEmitter()), this.onData = this._onData.event, this._onLineFeed = this.register(new s.EventEmitter()), this.onLineFeed = this._onLineFeed.event, this._onResize = this.register(new s.EventEmitter()), this.onResize = this._onResize.event, this._onWriteParsed = this.register(new s.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event, this._onScroll = this.register(new s.EventEmitter()), this._instantiationService = new a.InstantiationService(), this.optionsService = this.register(new m.OptionsService(B)), this._instantiationService.setService(c.IOptionsService, this.optionsService), this._bufferService = this.register(this._instantiationService.createInstance(v.BufferService)), this._instantiationService.setService(c.IBufferService, this._bufferService), this._logService = this.register(this._instantiationService.createInstance(d.LogService)), this._instantiationService.setService(c.ILogService, this._logService), this.coreService = this.register(this._instantiationService.createInstance(l.CoreService)), this._instantiationService.setService(c.ICoreService, this.coreService), this.coreMouseService = this.register(this._instantiationService.createInstance(r.CoreMouseService)), this._instantiationService.setService(c.ICoreMouseService, this.coreMouseService), this.unicodeService = this.register(this._instantiationService.createInstance(e.UnicodeService)), this._instantiationService.setService(c.IUnicodeService, this.unicodeService), this._charsetService = this._instantiationService.createInstance(t.CharsetService), this._instantiationService.setService(c.ICharsetService, this._charsetService), this._oscLinkService = this._instantiationService.createInstance(S.OscLinkService), this._instantiationService.setService(c.IOscLinkService, this._oscLinkService), this._inputHandler = this.register(new g.InputHandler(this._bufferService, this._charsetService, this.coreService, this._logService, this.optionsService, this._oscLinkService, this.coreMouseService, this.unicodeService)), this.register((0, s.forwardEvent)(this._inputHandler.onLineFeed, this._onLineFeed)), this.register(this._inputHandler), this.register((0, s.forwardEvent)(this._bufferService.onResize, this._onResize)), this.register((0, s.forwardEvent)(this.coreService.onData, this._onData)), this.register((0, s.forwardEvent)(this.coreService.onBinary, this._onBinary)), this.register(this.coreService.onRequestScrollToBottom(() => this.scrollToBottom())), this.register(this.coreService.onUserInput(() => this._writeBuffer.handleUserInput())), this.register(this.optionsService.onMultipleOptionChange(["windowsMode", "windowsPty"], () => this._handleWindowsPtyOptionChange())), this.register(this._bufferService.onScroll((T) => {
                                 this._onScroll.fire({
                                     position: this._bufferService.buffer.ydisp,
                                     source: 0
                                 }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom);
-                            })), this.register(this._inputHandler.onScroll((x) => {
+                            })), this.register(this._inputHandler.onScroll((T) => {
                                 this._onScroll.fire({
                                     position: this._bufferService.buffer.ydisp,
                                     source: 0
                                 }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom);
-                            })), this._writeBuffer = this.register(new u.WriteBuffer((x, L) => this._inputHandler.parse(x, L))), this.register((0, s.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed));
+                            })), this._writeBuffer = this.register(new u.WriteBuffer((T, L) => this._inputHandler.parse(T, L))), this.register((0, s.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed));
                         }
-                        write(T, x) {
-                            this._writeBuffer.write(T, x);
+                        write(B, T) {
+                            this._writeBuffer.write(B, T);
                         }
-                        writeSync(T, x) {
-                            this._logService.logLevel <= c.LogLevelEnum.WARN && !_ && (this._logService.warn("writeSync is unreliable and will be removed soon."), _ = !0), this._writeBuffer.writeSync(T, x);
+                        writeSync(B, T) {
+                            this._logService.logLevel <= c.LogLevelEnum.WARN && !_ && (this._logService.warn("writeSync is unreliable and will be removed soon."), _ = !0), this._writeBuffer.writeSync(B, T);
                         }
-                        input(T, x = !0) {
-                            this.coreService.triggerDataEvent(T, x);
+                        input(B, T = !0) {
+                            this.coreService.triggerDataEvent(B, T);
                         }
-                        resize(T, x) {
-                            isNaN(T) || isNaN(x) || (T = Math.max(T, f.MINIMUM_COLS), x = Math.max(x, f.MINIMUM_ROWS), this._bufferService.resize(T, x));
+                        resize(B, T) {
+                            isNaN(B) || isNaN(T) || (B = Math.max(B, v.MINIMUM_COLS), T = Math.max(T, v.MINIMUM_ROWS), this._bufferService.resize(B, T));
                         }
-                        scroll(T, x = !1) {
-                            this._bufferService.scroll(T, x);
+                        scroll(B, T = !1) {
+                            this._bufferService.scroll(B, T);
                         }
-                        scrollLines(T, x, L) {
-                            this._bufferService.scrollLines(T, x, L);
+                        scrollLines(B, T, L) {
+                            this._bufferService.scrollLines(B, T, L);
                         }
-                        scrollPages(T) {
-                            this.scrollLines(T * (this.rows - 1));
+                        scrollPages(B) {
+                            this.scrollLines(B * (this.rows - 1));
                         }
                         scrollToTop() {
                             this.scrollLines(-this._bufferService.buffer.ydisp);
                         }
                         scrollToBottom() {
                             this.scrollLines(this._bufferService.buffer.ybase - this._bufferService.buffer.ydisp);
                         }
-                        scrollToLine(T) {
-                            const x = T - this._bufferService.buffer.ydisp;
-                            x !== 0 && this.scrollLines(x);
+                        scrollToLine(B) {
+                            const T = B - this._bufferService.buffer.ydisp;
+                            T !== 0 && this.scrollLines(T);
                         }
-                        registerEscHandler(T, x) {
-                            return this._inputHandler.registerEscHandler(T, x);
+                        registerEscHandler(B, T) {
+                            return this._inputHandler.registerEscHandler(B, T);
                         }
-                        registerDcsHandler(T, x) {
-                            return this._inputHandler.registerDcsHandler(T, x);
+                        registerDcsHandler(B, T) {
+                            return this._inputHandler.registerDcsHandler(B, T);
                         }
-                        registerCsiHandler(T, x) {
-                            return this._inputHandler.registerCsiHandler(T, x);
+                        registerCsiHandler(B, T) {
+                            return this._inputHandler.registerCsiHandler(B, T);
                         }
-                        registerOscHandler(T, x) {
-                            return this._inputHandler.registerOscHandler(T, x);
+                        registerOscHandler(B, T) {
+                            return this._inputHandler.registerOscHandler(B, T);
                         }
                         _setup() {
                             this._handleWindowsPtyOptionChange();
                         }
                         reset() {
                             this._inputHandler.reset(), this._bufferService.reset(), this._charsetService.reset(), this.coreService.reset(), this.coreMouseService.reset();
                         }
                         _handleWindowsPtyOptionChange() {
-                            let T = !1;
-                            const x = this.optionsService.rawOptions.windowsPty;
-                            x && x.buildNumber !== void 0 && x.buildNumber !== void 0 ? T = x.backend === "conpty" && x.buildNumber < 21376 : this.optionsService.rawOptions.windowsMode && (T = !0), T ? this._enableWindowsWrappingHeuristics() : this._windowsWrappingHeuristics.clear();
+                            let B = !1;
+                            const T = this.optionsService.rawOptions.windowsPty;
+                            T && T.buildNumber !== void 0 && T.buildNumber !== void 0 ? B = T.backend === "conpty" && T.buildNumber < 21376 : this.optionsService.rawOptions.windowsMode && (B = !0), B ? this._enableWindowsWrappingHeuristics() : this._windowsWrappingHeuristics.clear();
                         }
                         _enableWindowsWrappingHeuristics() {
                             if (!this._windowsWrappingHeuristics.value) {
-                                const T = [];
-                                T.push(this.onLineFeed(h.updateWindowsModeWrappedState.bind(null, this._bufferService))), T.push(this.registerCsiHandler({
+                                const B = [];
+                                B.push(this.onLineFeed(h.updateWindowsModeWrappedState.bind(null, this._bufferService))), B.push(this.registerCsiHandler({
                                     final: "H"
                                 }, () => ((0, h.updateWindowsModeWrappedState)(this._bufferService), !1))), this._windowsWrappingHeuristics.value = (0, o.toDisposable)(() => {
-                                    for (const x of T)
-                                        x.dispose();
+                                    for (const T of B)
+                                        T.dispose();
                                 });
                             }
                         }
                     }
                     i.CoreTerminal = b;
                 },
                 8460: (k, i) => {
@@ -5880,61 +5880,61 @@
                     }, i.forwardEvent = function(n, o) {
                         return n((c) => o.fire(c));
                     }, i.runAndSubscribe = function(n, o) {
                         return o(void 0), n((c) => o(c));
                     };
                 },
                 5435: function(k, i, n) {
-                    var o = this && this.__decorate || function(j, C, D, B) {
+                    var o = this && this.__decorate || function(z, C, x, A) {
                             var O, I = arguments.length,
-                                z = I < 3 ? C : B === null ? B = Object.getOwnPropertyDescriptor(C, D) : B;
+                                q = I < 3 ? C : A === null ? A = Object.getOwnPropertyDescriptor(C, x) : A;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                z = Reflect.decorate(j, C, D, B);
+                                q = Reflect.decorate(z, C, x, A);
                             else
-                                for (var G = j.length - 1; G >= 0; G--)
-                                    (O = j[G]) && (z = (I < 3 ? O(z) : I > 3 ? O(C, D, z) : O(C, D)) || z);
-                            return I > 3 && z && Object.defineProperty(C, D, z), z;
+                                for (var X = z.length - 1; X >= 0; X--)
+                                    (O = z[X]) && (q = (I < 3 ? O(q) : I > 3 ? O(C, x, q) : O(C, x)) || q);
+                            return I > 3 && q && Object.defineProperty(C, x, q), q;
                         },
-                        c = this && this.__param || function(j, C) {
-                            return function(D, B) {
-                                C(D, B, j);
+                        c = this && this.__param || function(z, C) {
+                            return function(x, A) {
+                                C(x, A, z);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.InputHandler = i.WindowsOptionsReportType = void 0;
                     const a = n(2584),
                         d = n(7116),
-                        f = n(2015),
-                        g = n(844),
+                        v = n(2015),
+                        m = n(844),
                         l = n(482),
                         s = n(8437),
                         r = n(8460),
-                        t = n(643),
-                        e = n(511),
+                        e = n(643),
+                        t = n(511),
                         h = n(3734),
-                        v = n(2585),
+                        g = n(2585),
                         u = n(1480),
-                        p = n(6242),
+                        S = n(6242),
                         _ = n(6351),
                         b = n(5941),
-                        A = {
+                        R = {
                             "(": 0,
                             ")": 1,
                             "*": 2,
                             "+": 3,
                             "-": 1,
                             ".": 2
                         },
-                        T = 131072;
+                        B = 131072;
 
-                    function x(j, C) {
-                        if (j > 24)
+                    function T(z, C) {
+                        if (z > 24)
                             return C.setWinLines || !1;
-                        switch (j) {
+                        switch (z) {
                             case 1:
                                 return !!C.restoreWin;
                             case 2:
                                 return !!C.minimizeWin;
                             case 3:
                                 return !!C.setWinPosition;
                             case 4:
@@ -5975,55 +5975,55 @@
                                 return !!C.popTitle;
                             case 24:
                                 return !!C.setWinLines;
                         }
                         return !1;
                     }
                     var L;
-                    (function(j) {
-                        j[j.GET_WIN_SIZE_PIXELS = 0] = "GET_WIN_SIZE_PIXELS", j[j.GET_CELL_SIZE_PIXELS = 1] = "GET_CELL_SIZE_PIXELS";
+                    (function(z) {
+                        z[z.GET_WIN_SIZE_PIXELS = 0] = "GET_WIN_SIZE_PIXELS", z[z.GET_CELL_SIZE_PIXELS = 1] = "GET_CELL_SIZE_PIXELS";
                     })(L || (i.WindowsOptionsReportType = L = {}));
                     let H = 0;
-                    class W extends g.Disposable {
+                    class W extends m.Disposable {
                         getAttrData() {
                             return this._curAttrData;
                         }
-                        constructor(C, D, B, O, I, z, G, X, P = new f.EscapeSequenceParser()) {
-                            super(), this._bufferService = C, this._charsetService = D, this._coreService = B, this._logService = O, this._optionsService = I, this._oscLinkService = z, this._coreMouseService = G, this._unicodeService = X, this._parser = P, this._parseBuffer = new Uint32Array(4096), this._stringDecoder = new l.StringToUtf32(), this._utf8Decoder = new l.Utf8ToUtf32(), this._workCell = new e.CellData(), this._windowTitle = "", this._iconName = "", this._windowTitleStack = [], this._iconNameStack = [], this._curAttrData = s.DEFAULT_ATTR_DATA.clone(), this._eraseAttrDataInternal = s.DEFAULT_ATTR_DATA.clone(), this._onRequestBell = this.register(new r.EventEmitter()), this.onRequestBell = this._onRequestBell.event, this._onRequestRefreshRows = this.register(new r.EventEmitter()), this.onRequestRefreshRows = this._onRequestRefreshRows.event, this._onRequestReset = this.register(new r.EventEmitter()), this.onRequestReset = this._onRequestReset.event, this._onRequestSendFocus = this.register(new r.EventEmitter()), this.onRequestSendFocus = this._onRequestSendFocus.event, this._onRequestSyncScrollBar = this.register(new r.EventEmitter()), this.onRequestSyncScrollBar = this._onRequestSyncScrollBar.event, this._onRequestWindowsOptionsReport = this.register(new r.EventEmitter()), this.onRequestWindowsOptionsReport = this._onRequestWindowsOptionsReport.event, this._onA11yChar = this.register(new r.EventEmitter()), this.onA11yChar = this._onA11yChar.event, this._onA11yTab = this.register(new r.EventEmitter()), this.onA11yTab = this._onA11yTab.event, this._onCursorMove = this.register(new r.EventEmitter()), this.onCursorMove = this._onCursorMove.event, this._onLineFeed = this.register(new r.EventEmitter()), this.onLineFeed = this._onLineFeed.event, this._onScroll = this.register(new r.EventEmitter()), this.onScroll = this._onScroll.event, this._onTitleChange = this.register(new r.EventEmitter()), this.onTitleChange = this._onTitleChange.event, this._onColor = this.register(new r.EventEmitter()), this.onColor = this._onColor.event, this._parseStack = {
+                        constructor(C, x, A, O, I, q, X, J, P = new v.EscapeSequenceParser()) {
+                            super(), this._bufferService = C, this._charsetService = x, this._coreService = A, this._logService = O, this._optionsService = I, this._oscLinkService = q, this._coreMouseService = X, this._unicodeService = J, this._parser = P, this._parseBuffer = new Uint32Array(4096), this._stringDecoder = new l.StringToUtf32(), this._utf8Decoder = new l.Utf8ToUtf32(), this._workCell = new t.CellData(), this._windowTitle = "", this._iconName = "", this._windowTitleStack = [], this._iconNameStack = [], this._curAttrData = s.DEFAULT_ATTR_DATA.clone(), this._eraseAttrDataInternal = s.DEFAULT_ATTR_DATA.clone(), this._onRequestBell = this.register(new r.EventEmitter()), this.onRequestBell = this._onRequestBell.event, this._onRequestRefreshRows = this.register(new r.EventEmitter()), this.onRequestRefreshRows = this._onRequestRefreshRows.event, this._onRequestReset = this.register(new r.EventEmitter()), this.onRequestReset = this._onRequestReset.event, this._onRequestSendFocus = this.register(new r.EventEmitter()), this.onRequestSendFocus = this._onRequestSendFocus.event, this._onRequestSyncScrollBar = this.register(new r.EventEmitter()), this.onRequestSyncScrollBar = this._onRequestSyncScrollBar.event, this._onRequestWindowsOptionsReport = this.register(new r.EventEmitter()), this.onRequestWindowsOptionsReport = this._onRequestWindowsOptionsReport.event, this._onA11yChar = this.register(new r.EventEmitter()), this.onA11yChar = this._onA11yChar.event, this._onA11yTab = this.register(new r.EventEmitter()), this.onA11yTab = this._onA11yTab.event, this._onCursorMove = this.register(new r.EventEmitter()), this.onCursorMove = this._onCursorMove.event, this._onLineFeed = this.register(new r.EventEmitter()), this.onLineFeed = this._onLineFeed.event, this._onScroll = this.register(new r.EventEmitter()), this.onScroll = this._onScroll.event, this._onTitleChange = this.register(new r.EventEmitter()), this.onTitleChange = this._onTitleChange.event, this._onColor = this.register(new r.EventEmitter()), this.onColor = this._onColor.event, this._parseStack = {
                                 paused: !1,
                                 cursorStartX: 0,
                                 cursorStartY: 0,
                                 decodedLength: 0,
                                 position: 0
-                            }, this._specialColors = [256, 257, 258], this.register(this._parser), this._dirtyRowTracker = new U(this._bufferService), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate((w) => this._activeBuffer = w.activeBuffer)), this._parser.setCsiHandlerFallback((w, N) => {
+                            }, this._specialColors = [256, 257, 258], this.register(this._parser), this._dirtyRowTracker = new j(this._bufferService), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate((w) => this._activeBuffer = w.activeBuffer)), this._parser.setCsiHandlerFallback((w, U) => {
                                 this._logService.debug("Unknown CSI code: ", {
                                     identifier: this._parser.identToString(w),
-                                    params: N.toArray()
+                                    params: U.toArray()
                                 });
                             }), this._parser.setEscHandlerFallback((w) => {
                                 this._logService.debug("Unknown ESC code: ", {
                                     identifier: this._parser.identToString(w)
                                 });
                             }), this._parser.setExecuteHandlerFallback((w) => {
                                 this._logService.debug("Unknown EXECUTE code: ", {
                                     code: w
                                 });
-                            }), this._parser.setOscHandlerFallback((w, N, F) => {
+                            }), this._parser.setOscHandlerFallback((w, U, F) => {
                                 this._logService.debug("Unknown OSC code: ", {
                                     identifier: w,
-                                    action: N,
+                                    action: U,
                                     data: F
                                 });
-                            }), this._parser.setDcsHandlerFallback((w, N, F) => {
-                                N === "HOOK" && (F = F.toArray()), this._logService.debug("Unknown DCS code: ", {
+                            }), this._parser.setDcsHandlerFallback((w, U, F) => {
+                                U === "HOOK" && (F = F.toArray()), this._logService.debug("Unknown DCS code: ", {
                                     identifier: this._parser.identToString(w),
-                                    action: N,
+                                    action: U,
                                     payload: F
                                 });
-                            }), this._parser.setPrintHandler((w, N, F) => this.print(w, N, F)), this._parser.registerCsiHandler({
+                            }), this._parser.setPrintHandler((w, U, F) => this.print(w, U, F)), this._parser.registerCsiHandler({
                                 final: "@"
                             }, (w) => this.insertChars(w)), this._parser.registerCsiHandler({
                                 intermediates: " ",
                                 final: "@"
                             }, (w) => this.scrollLeft(w)), this._parser.registerCsiHandler({
                                 final: "A"
                             }, (w) => this.cursorUp(w)), this._parser.registerCsiHandler({
@@ -6131,15 +6131,15 @@
                             }, (w) => this.selectProtected(w)), this._parser.registerCsiHandler({
                                 intermediates: "$",
                                 final: "p"
                             }, (w) => this.requestMode(w, !0)), this._parser.registerCsiHandler({
                                 prefix: "?",
                                 intermediates: "$",
                                 final: "p"
-                            }, (w) => this.requestMode(w, !1)), this._parser.setExecuteHandler(a.C0.BEL, () => this.bell()), this._parser.setExecuteHandler(a.C0.LF, () => this.lineFeed()), this._parser.setExecuteHandler(a.C0.VT, () => this.lineFeed()), this._parser.setExecuteHandler(a.C0.FF, () => this.lineFeed()), this._parser.setExecuteHandler(a.C0.CR, () => this.carriageReturn()), this._parser.setExecuteHandler(a.C0.BS, () => this.backspace()), this._parser.setExecuteHandler(a.C0.HT, () => this.tab()), this._parser.setExecuteHandler(a.C0.SO, () => this.shiftOut()), this._parser.setExecuteHandler(a.C0.SI, () => this.shiftIn()), this._parser.setExecuteHandler(a.C1.IND, () => this.index()), this._parser.setExecuteHandler(a.C1.NEL, () => this.nextLine()), this._parser.setExecuteHandler(a.C1.HTS, () => this.tabSet()), this._parser.registerOscHandler(0, new p.OscHandler((w) => (this.setTitle(w), this.setIconName(w), !0))), this._parser.registerOscHandler(1, new p.OscHandler((w) => this.setIconName(w))), this._parser.registerOscHandler(2, new p.OscHandler((w) => this.setTitle(w))), this._parser.registerOscHandler(4, new p.OscHandler((w) => this.setOrReportIndexedColor(w))), this._parser.registerOscHandler(8, new p.OscHandler((w) => this.setHyperlink(w))), this._parser.registerOscHandler(10, new p.OscHandler((w) => this.setOrReportFgColor(w))), this._parser.registerOscHandler(11, new p.OscHandler((w) => this.setOrReportBgColor(w))), this._parser.registerOscHandler(12, new p.OscHandler((w) => this.setOrReportCursorColor(w))), this._parser.registerOscHandler(104, new p.OscHandler((w) => this.restoreIndexedColor(w))), this._parser.registerOscHandler(110, new p.OscHandler((w) => this.restoreFgColor(w))), this._parser.registerOscHandler(111, new p.OscHandler((w) => this.restoreBgColor(w))), this._parser.registerOscHandler(112, new p.OscHandler((w) => this.restoreCursorColor(w))), this._parser.registerEscHandler({
+                            }, (w) => this.requestMode(w, !1)), this._parser.setExecuteHandler(a.C0.BEL, () => this.bell()), this._parser.setExecuteHandler(a.C0.LF, () => this.lineFeed()), this._parser.setExecuteHandler(a.C0.VT, () => this.lineFeed()), this._parser.setExecuteHandler(a.C0.FF, () => this.lineFeed()), this._parser.setExecuteHandler(a.C0.CR, () => this.carriageReturn()), this._parser.setExecuteHandler(a.C0.BS, () => this.backspace()), this._parser.setExecuteHandler(a.C0.HT, () => this.tab()), this._parser.setExecuteHandler(a.C0.SO, () => this.shiftOut()), this._parser.setExecuteHandler(a.C0.SI, () => this.shiftIn()), this._parser.setExecuteHandler(a.C1.IND, () => this.index()), this._parser.setExecuteHandler(a.C1.NEL, () => this.nextLine()), this._parser.setExecuteHandler(a.C1.HTS, () => this.tabSet()), this._parser.registerOscHandler(0, new S.OscHandler((w) => (this.setTitle(w), this.setIconName(w), !0))), this._parser.registerOscHandler(1, new S.OscHandler((w) => this.setIconName(w))), this._parser.registerOscHandler(2, new S.OscHandler((w) => this.setTitle(w))), this._parser.registerOscHandler(4, new S.OscHandler((w) => this.setOrReportIndexedColor(w))), this._parser.registerOscHandler(8, new S.OscHandler((w) => this.setHyperlink(w))), this._parser.registerOscHandler(10, new S.OscHandler((w) => this.setOrReportFgColor(w))), this._parser.registerOscHandler(11, new S.OscHandler((w) => this.setOrReportBgColor(w))), this._parser.registerOscHandler(12, new S.OscHandler((w) => this.setOrReportCursorColor(w))), this._parser.registerOscHandler(104, new S.OscHandler((w) => this.restoreIndexedColor(w))), this._parser.registerOscHandler(110, new S.OscHandler((w) => this.restoreFgColor(w))), this._parser.registerOscHandler(111, new S.OscHandler((w) => this.restoreBgColor(w))), this._parser.registerOscHandler(112, new S.OscHandler((w) => this.restoreCursorColor(w))), this._parser.registerEscHandler({
                                 final: "7"
                             }, () => this.saveCursor()), this._parser.registerEscHandler({
                                 final: "8"
                             }, () => this.restoreCursor()), this._parser.registerEscHandler({
                                 final: "D"
                             }, () => this.index()), this._parser.registerEscHandler({
                                 final: "E"
@@ -6195,107 +6195,107 @@
                                 }, () => this.selectCharset("/" + w));
                             this._parser.registerEscHandler({
                                 intermediates: "#",
                                 final: "8"
                             }, () => this.screenAlignmentPattern()), this._parser.setErrorHandler((w) => (this._logService.error("Parsing error: ", w), w)), this._parser.registerDcsHandler({
                                 intermediates: "$",
                                 final: "q"
-                            }, new _.DcsHandler((w, N) => this.requestStatusString(w, N)));
+                            }, new _.DcsHandler((w, U) => this.requestStatusString(w, U)));
                         }
-                        _preserveStack(C, D, B, O) {
-                            this._parseStack.paused = !0, this._parseStack.cursorStartX = C, this._parseStack.cursorStartY = D, this._parseStack.decodedLength = B, this._parseStack.position = O;
+                        _preserveStack(C, x, A, O) {
+                            this._parseStack.paused = !0, this._parseStack.cursorStartX = C, this._parseStack.cursorStartY = x, this._parseStack.decodedLength = A, this._parseStack.position = O;
                         }
                         _logSlowResolvingAsync(C) {
-                            this._logService.logLevel <= v.LogLevelEnum.WARN && Promise.race([C, new Promise((D, B) => setTimeout(() => B("#SLOW_TIMEOUT"), 5e3))]).catch((D) => {
-                                if (D !== "#SLOW_TIMEOUT")
-                                    throw D;
+                            this._logService.logLevel <= g.LogLevelEnum.WARN && Promise.race([C, new Promise((x, A) => setTimeout(() => A("#SLOW_TIMEOUT"), 5e3))]).catch((x) => {
+                                if (x !== "#SLOW_TIMEOUT")
+                                    throw x;
                                 console.warn("async parser handler taking longer than 5000 ms");
                             });
                         }
                         _getCurrentLinkId() {
                             return this._curAttrData.extended.urlId;
                         }
-                        parse(C, D) {
-                            let B, O = this._activeBuffer.x,
+                        parse(C, x) {
+                            let A, O = this._activeBuffer.x,
                                 I = this._activeBuffer.y,
-                                z = 0;
-                            const G = this._parseStack.paused;
-                            if (G) {
-                                if (B = this._parser.parse(this._parseBuffer, this._parseStack.decodedLength, D))
-                                    return this._logSlowResolvingAsync(B), B;
-                                O = this._parseStack.cursorStartX, I = this._parseStack.cursorStartY, this._parseStack.paused = !1, C.length > T && (z = this._parseStack.position + T);
-                            }
-                            if (this._logService.logLevel <= v.LogLevelEnum.DEBUG && this._logService.debug("parsing data" + (typeof C == "string" ? ` "${C}"` : ` "${Array.prototype.map.call(C, (w) => String.fromCharCode(w)).join("")}"`), typeof C == "string" ? C.split("").map((w) => w.charCodeAt(0)) : C), this._parseBuffer.length < C.length && this._parseBuffer.length < T && (this._parseBuffer = new Uint32Array(Math.min(C.length, T))), G || this._dirtyRowTracker.clearRange(), C.length > T)
-                                for (let w = z; w < C.length; w += T) {
-                                    const N = w + T < C.length ? w + T : C.length,
-                                        F = typeof C == "string" ? this._stringDecoder.decode(C.substring(w, N), this._parseBuffer) : this._utf8Decoder.decode(C.subarray(w, N), this._parseBuffer);
-                                    if (B = this._parser.parse(this._parseBuffer, F))
-                                        return this._preserveStack(O, I, F, w), this._logSlowResolvingAsync(B), B;
+                                q = 0;
+                            const X = this._parseStack.paused;
+                            if (X) {
+                                if (A = this._parser.parse(this._parseBuffer, this._parseStack.decodedLength, x))
+                                    return this._logSlowResolvingAsync(A), A;
+                                O = this._parseStack.cursorStartX, I = this._parseStack.cursorStartY, this._parseStack.paused = !1, C.length > B && (q = this._parseStack.position + B);
+                            }
+                            if (this._logService.logLevel <= g.LogLevelEnum.DEBUG && this._logService.debug("parsing data" + (typeof C == "string" ? ` "${C}"` : ` "${Array.prototype.map.call(C, (w) => String.fromCharCode(w)).join("")}"`), typeof C == "string" ? C.split("").map((w) => w.charCodeAt(0)) : C), this._parseBuffer.length < C.length && this._parseBuffer.length < B && (this._parseBuffer = new Uint32Array(Math.min(C.length, B))), X || this._dirtyRowTracker.clearRange(), C.length > B)
+                                for (let w = q; w < C.length; w += B) {
+                                    const U = w + B < C.length ? w + B : C.length,
+                                        F = typeof C == "string" ? this._stringDecoder.decode(C.substring(w, U), this._parseBuffer) : this._utf8Decoder.decode(C.subarray(w, U), this._parseBuffer);
+                                    if (A = this._parser.parse(this._parseBuffer, F))
+                                        return this._preserveStack(O, I, F, w), this._logSlowResolvingAsync(A), A;
                                 }
-                            else if (!G) {
+                            else if (!X) {
                                 const w = typeof C == "string" ? this._stringDecoder.decode(C, this._parseBuffer) : this._utf8Decoder.decode(C, this._parseBuffer);
-                                if (B = this._parser.parse(this._parseBuffer, w))
-                                    return this._preserveStack(O, I, w, 0), this._logSlowResolvingAsync(B), B;
+                                if (A = this._parser.parse(this._parseBuffer, w))
+                                    return this._preserveStack(O, I, w, 0), this._logSlowResolvingAsync(A), A;
                             }
                             this._activeBuffer.x === O && this._activeBuffer.y === I || this._onCursorMove.fire();
-                            const X = this._dirtyRowTracker.end + (this._bufferService.buffer.ybase - this._bufferService.buffer.ydisp),
+                            const J = this._dirtyRowTracker.end + (this._bufferService.buffer.ybase - this._bufferService.buffer.ydisp),
                                 P = this._dirtyRowTracker.start + (this._bufferService.buffer.ybase - this._bufferService.buffer.ydisp);
-                            P < this._bufferService.rows && this._onRequestRefreshRows.fire(Math.min(P, this._bufferService.rows - 1), Math.min(X, this._bufferService.rows - 1));
+                            P < this._bufferService.rows && this._onRequestRefreshRows.fire(Math.min(P, this._bufferService.rows - 1), Math.min(J, this._bufferService.rows - 1));
                         }
-                        print(C, D, B) {
+                        print(C, x, A) {
                             let O, I;
-                            const z = this._charsetService.charset,
-                                G = this._optionsService.rawOptions.screenReaderMode,
-                                X = this._bufferService.cols,
+                            const q = this._charsetService.charset,
+                                X = this._optionsService.rawOptions.screenReaderMode,
+                                J = this._bufferService.cols,
                                 P = this._coreService.decPrivateModes.wraparound,
                                 w = this._coreService.modes.insertMode,
-                                N = this._curAttrData;
+                                U = this._curAttrData;
                             let F = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                            this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._activeBuffer.x && B - D > 0 && F.getWidth(this._activeBuffer.x - 1) === 2 && F.setCellFromCodepoint(this._activeBuffer.x - 1, 0, 1, N);
-                            let V = this._parser.precedingJoinState;
-                            for (let q = D; q < B; ++q) {
-                                if (O = C[q], O < 127 && z) {
-                                    const re = z[String.fromCharCode(O)];
-                                    re && (O = re.charCodeAt(0));
-                                }
-                                const Z = this._unicodeService.charProperties(O, V);
-                                I = u.UnicodeService.extractWidth(Z);
-                                const ie = u.UnicodeService.extractShouldJoin(Z),
-                                    se = ie ? u.UnicodeService.extractWidth(V) : 0;
-                                if (V = Z, G && this._onA11yChar.fire((0, l.stringFromCodePoint)(O)), this._getCurrentLinkId() && this._oscLinkService.addLineToLink(this._getCurrentLinkId(), this._activeBuffer.ybase + this._activeBuffer.y), this._activeBuffer.x + I - se > X) {
+                            this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._activeBuffer.x && A - x > 0 && F.getWidth(this._activeBuffer.x - 1) === 2 && F.setCellFromCodepoint(this._activeBuffer.x - 1, 0, 1, U);
+                            let G = this._parser.precedingJoinState;
+                            for (let K = x; K < A; ++K) {
+                                if (O = C[K], O < 127 && q) {
+                                    const oe = q[String.fromCharCode(O)];
+                                    oe && (O = oe.charCodeAt(0));
+                                }
+                                const ee = this._unicodeService.charProperties(O, G);
+                                I = u.UnicodeService.extractWidth(ee);
+                                const se = u.UnicodeService.extractShouldJoin(ee),
+                                    ie = se ? u.UnicodeService.extractWidth(G) : 0;
+                                if (G = ee, X && this._onA11yChar.fire((0, l.stringFromCodePoint)(O)), this._getCurrentLinkId() && this._oscLinkService.addLineToLink(this._getCurrentLinkId(), this._activeBuffer.ybase + this._activeBuffer.y), this._activeBuffer.x + I - ie > J) {
                                     if (P) {
-                                        const re = F;
-                                        let J = this._activeBuffer.x - se;
-                                        for (this._activeBuffer.x = se, this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData(), !0)) : (this._activeBuffer.y >= this._bufferService.rows && (this._activeBuffer.y = this._bufferService.rows - 1), this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !0), F = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y), se > 0 && F instanceof s.BufferLine && F.copyCellsFrom(re, J, 0, se, !1); J < X;)
-                                            re.setCellFromCodepoint(J++, 0, 1, N);
-                                    } else if (this._activeBuffer.x = X - 1, I === 2)
+                                        const oe = F;
+                                        let Z = this._activeBuffer.x - ie;
+                                        for (this._activeBuffer.x = ie, this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData(), !0)) : (this._activeBuffer.y >= this._bufferService.rows && (this._activeBuffer.y = this._bufferService.rows - 1), this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !0), F = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y), ie > 0 && F instanceof s.BufferLine && F.copyCellsFrom(oe, Z, 0, ie, !1); Z < J;)
+                                            oe.setCellFromCodepoint(Z++, 0, 1, U);
+                                    } else if (this._activeBuffer.x = J - 1, I === 2)
                                         continue;
                                 }
-                                if (ie && this._activeBuffer.x) {
-                                    const re = F.getWidth(this._activeBuffer.x - 1) ? 1 : 2;
-                                    F.addCodepointToCell(this._activeBuffer.x - re, O, I);
-                                    for (let J = I - se; --J >= 0;)
-                                        F.setCellFromCodepoint(this._activeBuffer.x++, 0, 0, N);
-                                } else if (w && (F.insertCells(this._activeBuffer.x, I - se, this._activeBuffer.getNullCell(N)), F.getWidth(X - 1) === 2 && F.setCellFromCodepoint(X - 1, t.NULL_CELL_CODE, t.NULL_CELL_WIDTH, N)), F.setCellFromCodepoint(this._activeBuffer.x++, O, I, N), I > 0)
+                                if (se && this._activeBuffer.x) {
+                                    const oe = F.getWidth(this._activeBuffer.x - 1) ? 1 : 2;
+                                    F.addCodepointToCell(this._activeBuffer.x - oe, O, I);
+                                    for (let Z = I - ie; --Z >= 0;)
+                                        F.setCellFromCodepoint(this._activeBuffer.x++, 0, 0, U);
+                                } else if (w && (F.insertCells(this._activeBuffer.x, I - ie, this._activeBuffer.getNullCell(U)), F.getWidth(J - 1) === 2 && F.setCellFromCodepoint(J - 1, e.NULL_CELL_CODE, e.NULL_CELL_WIDTH, U)), F.setCellFromCodepoint(this._activeBuffer.x++, O, I, U), I > 0)
                                     for (; --I;)
-                                        F.setCellFromCodepoint(this._activeBuffer.x++, 0, 0, N);
+                                        F.setCellFromCodepoint(this._activeBuffer.x++, 0, 0, U);
                             }
-                            this._parser.precedingJoinState = V, this._activeBuffer.x < X && B - D > 0 && F.getWidth(this._activeBuffer.x) === 0 && !F.hasContent(this._activeBuffer.x) && F.setCellFromCodepoint(this._activeBuffer.x, 0, 1, N), this._dirtyRowTracker.markDirty(this._activeBuffer.y);
+                            this._parser.precedingJoinState = G, this._activeBuffer.x < J && A - x > 0 && F.getWidth(this._activeBuffer.x) === 0 && !F.hasContent(this._activeBuffer.x) && F.setCellFromCodepoint(this._activeBuffer.x, 0, 1, U), this._dirtyRowTracker.markDirty(this._activeBuffer.y);
                         }
-                        registerCsiHandler(C, D) {
-                            return C.final !== "t" || C.prefix || C.intermediates ? this._parser.registerCsiHandler(C, D) : this._parser.registerCsiHandler(C, (B) => !x(B.params[0], this._optionsService.rawOptions.windowOptions) || D(B));
+                        registerCsiHandler(C, x) {
+                            return C.final !== "t" || C.prefix || C.intermediates ? this._parser.registerCsiHandler(C, x) : this._parser.registerCsiHandler(C, (A) => !T(A.params[0], this._optionsService.rawOptions.windowOptions) || x(A));
                         }
-                        registerDcsHandler(C, D) {
-                            return this._parser.registerDcsHandler(C, new _.DcsHandler(D));
+                        registerDcsHandler(C, x) {
+                            return this._parser.registerDcsHandler(C, new _.DcsHandler(x));
                         }
-                        registerEscHandler(C, D) {
-                            return this._parser.registerEscHandler(C, D);
+                        registerEscHandler(C, x) {
+                            return this._parser.registerEscHandler(C, x);
                         }
-                        registerOscHandler(C, D) {
-                            return this._parser.registerOscHandler(C, new p.OscHandler(D));
+                        registerOscHandler(C, x) {
+                            return this._parser.registerOscHandler(C, new S.OscHandler(x));
                         }
                         bell() {
                             return this._onRequestBell.fire(), !0;
                         }
                         lineFeed() {
                             return this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._optionsService.rawOptions.convertEol && (this._activeBuffer.x = 0), this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData())) : this._activeBuffer.y >= this._bufferService.rows ? this._activeBuffer.y = this._bufferService.rows - 1 : this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !1, this._activeBuffer.x >= this._bufferService.cols && this._activeBuffer.x--, this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._onLineFeed.fire(), !0;
                         }
@@ -6306,16 +6306,16 @@
                             var C;
                             if (!this._coreService.decPrivateModes.reverseWraparound)
                                 return this._restrictCursor(), this._activeBuffer.x > 0 && this._activeBuffer.x--, !0;
                             if (this._restrictCursor(this._bufferService.cols), this._activeBuffer.x > 0)
                                 this._activeBuffer.x--;
                             else if (this._activeBuffer.x === 0 && this._activeBuffer.y > this._activeBuffer.scrollTop && this._activeBuffer.y <= this._activeBuffer.scrollBottom && ((C = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y)) != null && C.isWrapped)) {
                                 this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !1, this._activeBuffer.y--, this._activeBuffer.x = this._bufferService.cols - 1;
-                                const D = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                                D.hasWidth(this._activeBuffer.x) && !D.hasContent(this._activeBuffer.x) && this._activeBuffer.x--;
+                                const x = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
+                                x.hasWidth(this._activeBuffer.x) && !x.hasContent(this._activeBuffer.x) && this._activeBuffer.x--;
                             }
                             return this._restrictCursor(), !0;
                         }
                         tab() {
                             if (this._activeBuffer.x >= this._bufferService.cols)
                                 return !0;
                             const C = this._activeBuffer.x;
@@ -6326,27 +6326,27 @@
                         }
                         shiftIn() {
                             return this._charsetService.setgLevel(0), !0;
                         }
                         _restrictCursor(C = this._bufferService.cols - 1) {
                             this._activeBuffer.x = Math.min(C, Math.max(0, this._activeBuffer.x)), this._activeBuffer.y = this._coreService.decPrivateModes.origin ? Math.min(this._activeBuffer.scrollBottom, Math.max(this._activeBuffer.scrollTop, this._activeBuffer.y)) : Math.min(this._bufferService.rows - 1, Math.max(0, this._activeBuffer.y)), this._dirtyRowTracker.markDirty(this._activeBuffer.y);
                         }
-                        _setCursor(C, D) {
-                            this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._coreService.decPrivateModes.origin ? (this._activeBuffer.x = C, this._activeBuffer.y = this._activeBuffer.scrollTop + D) : (this._activeBuffer.x = C, this._activeBuffer.y = D), this._restrictCursor(), this._dirtyRowTracker.markDirty(this._activeBuffer.y);
+                        _setCursor(C, x) {
+                            this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._coreService.decPrivateModes.origin ? (this._activeBuffer.x = C, this._activeBuffer.y = this._activeBuffer.scrollTop + x) : (this._activeBuffer.x = C, this._activeBuffer.y = x), this._restrictCursor(), this._dirtyRowTracker.markDirty(this._activeBuffer.y);
                         }
-                        _moveCursor(C, D) {
-                            this._restrictCursor(), this._setCursor(this._activeBuffer.x + C, this._activeBuffer.y + D);
+                        _moveCursor(C, x) {
+                            this._restrictCursor(), this._setCursor(this._activeBuffer.x + C, this._activeBuffer.y + x);
                         }
                         cursorUp(C) {
-                            const D = this._activeBuffer.y - this._activeBuffer.scrollTop;
-                            return D >= 0 ? this._moveCursor(0, -Math.min(D, C.params[0] || 1)) : this._moveCursor(0, -(C.params[0] || 1)), !0;
+                            const x = this._activeBuffer.y - this._activeBuffer.scrollTop;
+                            return x >= 0 ? this._moveCursor(0, -Math.min(x, C.params[0] || 1)) : this._moveCursor(0, -(C.params[0] || 1)), !0;
                         }
                         cursorDown(C) {
-                            const D = this._activeBuffer.scrollBottom - this._activeBuffer.y;
-                            return D >= 0 ? this._moveCursor(0, Math.min(D, C.params[0] || 1)) : this._moveCursor(0, C.params[0] || 1), !0;
+                            const x = this._activeBuffer.scrollBottom - this._activeBuffer.y;
+                            return x >= 0 ? this._moveCursor(0, Math.min(x, C.params[0] || 1)) : this._moveCursor(0, C.params[0] || 1), !0;
                         }
                         cursorForward(C) {
                             return this._moveCursor(C.params[0] || 1, 0), !0;
                         }
                         cursorBackward(C) {
                             return this._moveCursor(-(C.params[0] || 1), 0), !0;
                         }
@@ -6374,214 +6374,214 @@
                         vPositionRelative(C) {
                             return this._moveCursor(0, C.params[0] || 1), !0;
                         }
                         hVPosition(C) {
                             return this.cursorPosition(C), !0;
                         }
                         tabClear(C) {
-                            const D = C.params[0];
-                            return D === 0 ? delete this._activeBuffer.tabs[this._activeBuffer.x] : D === 3 && (this._activeBuffer.tabs = {}), !0;
+                            const x = C.params[0];
+                            return x === 0 ? delete this._activeBuffer.tabs[this._activeBuffer.x] : x === 3 && (this._activeBuffer.tabs = {}), !0;
                         }
                         cursorForwardTab(C) {
                             if (this._activeBuffer.x >= this._bufferService.cols)
                                 return !0;
-                            let D = C.params[0] || 1;
-                            for (; D--;)
+                            let x = C.params[0] || 1;
+                            for (; x--;)
                                 this._activeBuffer.x = this._activeBuffer.nextStop();
                             return !0;
                         }
                         cursorBackwardTab(C) {
                             if (this._activeBuffer.x >= this._bufferService.cols)
                                 return !0;
-                            let D = C.params[0] || 1;
-                            for (; D--;)
+                            let x = C.params[0] || 1;
+                            for (; x--;)
                                 this._activeBuffer.x = this._activeBuffer.prevStop();
                             return !0;
                         }
                         selectProtected(C) {
-                            const D = C.params[0];
-                            return D === 1 && (this._curAttrData.bg |= 536870912), D !== 2 && D !== 0 || (this._curAttrData.bg &= -536870913), !0;
+                            const x = C.params[0];
+                            return x === 1 && (this._curAttrData.bg |= 536870912), x !== 2 && x !== 0 || (this._curAttrData.bg &= -536870913), !0;
                         }
-                        _eraseInBufferLine(C, D, B, O = !1, I = !1) {
-                            const z = this._activeBuffer.lines.get(this._activeBuffer.ybase + C);
-                            z.replaceCells(D, B, this._activeBuffer.getNullCell(this._eraseAttrData()), I), O && (z.isWrapped = !1);
-                        }
-                        _resetBufferLine(C, D = !1) {
-                            const B = this._activeBuffer.lines.get(this._activeBuffer.ybase + C);
-                            B && (B.fill(this._activeBuffer.getNullCell(this._eraseAttrData()), D), this._bufferService.buffer.clearMarkers(this._activeBuffer.ybase + C), B.isWrapped = !1);
+                        _eraseInBufferLine(C, x, A, O = !1, I = !1) {
+                            const q = this._activeBuffer.lines.get(this._activeBuffer.ybase + C);
+                            q.replaceCells(x, A, this._activeBuffer.getNullCell(this._eraseAttrData()), I), O && (q.isWrapped = !1);
+                        }
+                        _resetBufferLine(C, x = !1) {
+                            const A = this._activeBuffer.lines.get(this._activeBuffer.ybase + C);
+                            A && (A.fill(this._activeBuffer.getNullCell(this._eraseAttrData()), x), this._bufferService.buffer.clearMarkers(this._activeBuffer.ybase + C), A.isWrapped = !1);
                         }
-                        eraseInDisplay(C, D = !1) {
-                            let B;
+                        eraseInDisplay(C, x = !1) {
+                            let A;
                             switch (this._restrictCursor(this._bufferService.cols), C.params[0]) {
                                 case 0:
-                                    for (B = this._activeBuffer.y, this._dirtyRowTracker.markDirty(B), this._eraseInBufferLine(B++, this._activeBuffer.x, this._bufferService.cols, this._activeBuffer.x === 0, D); B < this._bufferService.rows; B++)
-                                        this._resetBufferLine(B, D);
-                                    this._dirtyRowTracker.markDirty(B);
+                                    for (A = this._activeBuffer.y, this._dirtyRowTracker.markDirty(A), this._eraseInBufferLine(A++, this._activeBuffer.x, this._bufferService.cols, this._activeBuffer.x === 0, x); A < this._bufferService.rows; A++)
+                                        this._resetBufferLine(A, x);
+                                    this._dirtyRowTracker.markDirty(A);
                                     break;
                                 case 1:
-                                    for (B = this._activeBuffer.y, this._dirtyRowTracker.markDirty(B), this._eraseInBufferLine(B, 0, this._activeBuffer.x + 1, !0, D), this._activeBuffer.x + 1 >= this._bufferService.cols && (this._activeBuffer.lines.get(B + 1).isWrapped = !1); B--;)
-                                        this._resetBufferLine(B, D);
+                                    for (A = this._activeBuffer.y, this._dirtyRowTracker.markDirty(A), this._eraseInBufferLine(A, 0, this._activeBuffer.x + 1, !0, x), this._activeBuffer.x + 1 >= this._bufferService.cols && (this._activeBuffer.lines.get(A + 1).isWrapped = !1); A--;)
+                                        this._resetBufferLine(A, x);
                                     this._dirtyRowTracker.markDirty(0);
                                     break;
                                 case 2:
-                                    for (B = this._bufferService.rows, this._dirtyRowTracker.markDirty(B - 1); B--;)
-                                        this._resetBufferLine(B, D);
+                                    for (A = this._bufferService.rows, this._dirtyRowTracker.markDirty(A - 1); A--;)
+                                        this._resetBufferLine(A, x);
                                     this._dirtyRowTracker.markDirty(0);
                                     break;
                                 case 3:
                                     const O = this._activeBuffer.lines.length - this._bufferService.rows;
                                     O > 0 && (this._activeBuffer.lines.trimStart(O), this._activeBuffer.ybase = Math.max(this._activeBuffer.ybase - O, 0), this._activeBuffer.ydisp = Math.max(this._activeBuffer.ydisp - O, 0), this._onScroll.fire(0));
                             }
                             return !0;
                         }
-                        eraseInLine(C, D = !1) {
+                        eraseInLine(C, x = !1) {
                             switch (this._restrictCursor(this._bufferService.cols), C.params[0]) {
                                 case 0:
-                                    this._eraseInBufferLine(this._activeBuffer.y, this._activeBuffer.x, this._bufferService.cols, this._activeBuffer.x === 0, D);
+                                    this._eraseInBufferLine(this._activeBuffer.y, this._activeBuffer.x, this._bufferService.cols, this._activeBuffer.x === 0, x);
                                     break;
                                 case 1:
-                                    this._eraseInBufferLine(this._activeBuffer.y, 0, this._activeBuffer.x + 1, !1, D);
+                                    this._eraseInBufferLine(this._activeBuffer.y, 0, this._activeBuffer.x + 1, !1, x);
                                     break;
                                 case 2:
-                                    this._eraseInBufferLine(this._activeBuffer.y, 0, this._bufferService.cols, !0, D);
+                                    this._eraseInBufferLine(this._activeBuffer.y, 0, this._bufferService.cols, !0, x);
                             }
                             return this._dirtyRowTracker.markDirty(this._activeBuffer.y), !0;
                         }
                         insertLines(C) {
                             this._restrictCursor();
-                            let D = C.params[0] || 1;
+                            let x = C.params[0] || 1;
                             if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop)
                                 return !0;
-                            const B = this._activeBuffer.ybase + this._activeBuffer.y,
+                            const A = this._activeBuffer.ybase + this._activeBuffer.y,
                                 O = this._bufferService.rows - 1 - this._activeBuffer.scrollBottom,
                                 I = this._bufferService.rows - 1 + this._activeBuffer.ybase - O + 1;
-                            for (; D--;)
-                                this._activeBuffer.lines.splice(I - 1, 1), this._activeBuffer.lines.splice(B, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
+                            for (; x--;)
+                                this._activeBuffer.lines.splice(I - 1, 1), this._activeBuffer.lines.splice(A, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.y, this._activeBuffer.scrollBottom), this._activeBuffer.x = 0, !0;
                         }
                         deleteLines(C) {
                             this._restrictCursor();
-                            let D = C.params[0] || 1;
+                            let x = C.params[0] || 1;
                             if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop)
                                 return !0;
-                            const B = this._activeBuffer.ybase + this._activeBuffer.y;
+                            const A = this._activeBuffer.ybase + this._activeBuffer.y;
                             let O;
-                            for (O = this._bufferService.rows - 1 - this._activeBuffer.scrollBottom, O = this._bufferService.rows - 1 + this._activeBuffer.ybase - O; D--;)
-                                this._activeBuffer.lines.splice(B, 1), this._activeBuffer.lines.splice(O, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
+                            for (O = this._bufferService.rows - 1 - this._activeBuffer.scrollBottom, O = this._bufferService.rows - 1 + this._activeBuffer.ybase - O; x--;)
+                                this._activeBuffer.lines.splice(A, 1), this._activeBuffer.lines.splice(O, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.y, this._activeBuffer.scrollBottom), this._activeBuffer.x = 0, !0;
                         }
                         insertChars(C) {
                             this._restrictCursor();
-                            const D = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                            return D && (D.insertCells(this._activeBuffer.x, C.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0;
+                            const x = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
+                            return x && (x.insertCells(this._activeBuffer.x, C.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0;
                         }
                         deleteChars(C) {
                             this._restrictCursor();
-                            const D = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                            return D && (D.deleteCells(this._activeBuffer.x, C.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0;
+                            const x = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
+                            return x && (x.deleteCells(this._activeBuffer.x, C.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0;
                         }
                         scrollUp(C) {
-                            let D = C.params[0] || 1;
-                            for (; D--;)
+                            let x = C.params[0] || 1;
+                            for (; x--;)
                                 this._activeBuffer.lines.splice(this._activeBuffer.ybase + this._activeBuffer.scrollTop, 1), this._activeBuffer.lines.splice(this._activeBuffer.ybase + this._activeBuffer.scrollBottom, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0;
                         }
                         scrollDown(C) {
-                            let D = C.params[0] || 1;
-                            for (; D--;)
+                            let x = C.params[0] || 1;
+                            for (; x--;)
                                 this._activeBuffer.lines.splice(this._activeBuffer.ybase + this._activeBuffer.scrollBottom, 1), this._activeBuffer.lines.splice(this._activeBuffer.ybase + this._activeBuffer.scrollTop, 0, this._activeBuffer.getBlankLine(s.DEFAULT_ATTR_DATA));
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0;
                         }
                         scrollLeft(C) {
                             if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop)
                                 return !0;
-                            const D = C.params[0] || 1;
-                            for (let B = this._activeBuffer.scrollTop; B <= this._activeBuffer.scrollBottom; ++B) {
-                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + B);
-                                O.deleteCells(0, D, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
+                            const x = C.params[0] || 1;
+                            for (let A = this._activeBuffer.scrollTop; A <= this._activeBuffer.scrollBottom; ++A) {
+                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + A);
+                                O.deleteCells(0, x, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
                             }
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0;
                         }
                         scrollRight(C) {
                             if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop)
                                 return !0;
-                            const D = C.params[0] || 1;
-                            for (let B = this._activeBuffer.scrollTop; B <= this._activeBuffer.scrollBottom; ++B) {
-                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + B);
-                                O.insertCells(0, D, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
+                            const x = C.params[0] || 1;
+                            for (let A = this._activeBuffer.scrollTop; A <= this._activeBuffer.scrollBottom; ++A) {
+                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + A);
+                                O.insertCells(0, x, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
                             }
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0;
                         }
                         insertColumns(C) {
                             if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop)
                                 return !0;
-                            const D = C.params[0] || 1;
-                            for (let B = this._activeBuffer.scrollTop; B <= this._activeBuffer.scrollBottom; ++B) {
-                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + B);
-                                O.insertCells(this._activeBuffer.x, D, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
+                            const x = C.params[0] || 1;
+                            for (let A = this._activeBuffer.scrollTop; A <= this._activeBuffer.scrollBottom; ++A) {
+                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + A);
+                                O.insertCells(this._activeBuffer.x, x, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
                             }
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0;
                         }
                         deleteColumns(C) {
                             if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop)
                                 return !0;
-                            const D = C.params[0] || 1;
-                            for (let B = this._activeBuffer.scrollTop; B <= this._activeBuffer.scrollBottom; ++B) {
-                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + B);
-                                O.deleteCells(this._activeBuffer.x, D, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
+                            const x = C.params[0] || 1;
+                            for (let A = this._activeBuffer.scrollTop; A <= this._activeBuffer.scrollBottom; ++A) {
+                                const O = this._activeBuffer.lines.get(this._activeBuffer.ybase + A);
+                                O.deleteCells(this._activeBuffer.x, x, this._activeBuffer.getNullCell(this._eraseAttrData())), O.isWrapped = !1;
                             }
                             return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0;
                         }
                         eraseChars(C) {
                             this._restrictCursor();
-                            const D = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                            return D && (D.replaceCells(this._activeBuffer.x, this._activeBuffer.x + (C.params[0] || 1), this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0;
+                            const x = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
+                            return x && (x.replaceCells(this._activeBuffer.x, this._activeBuffer.x + (C.params[0] || 1), this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0;
                         }
                         repeatPrecedingCharacter(C) {
-                            const D = this._parser.precedingJoinState;
-                            if (!D)
+                            const x = this._parser.precedingJoinState;
+                            if (!x)
                                 return !0;
-                            const B = C.params[0] || 1,
-                                O = u.UnicodeService.extractWidth(D),
+                            const A = C.params[0] || 1,
+                                O = u.UnicodeService.extractWidth(x),
                                 I = this._activeBuffer.x - O,
-                                z = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).getString(I),
-                                G = new Uint32Array(z.length * B);
-                            let X = 0;
-                            for (let w = 0; w < z.length;) {
-                                const N = z.codePointAt(w) || 0;
-                                G[X++] = N, w += N > 65535 ? 2 : 1;
-                            }
-                            let P = X;
-                            for (let w = 1; w < B; ++w)
-                                G.copyWithin(P, 0, X), P += X;
-                            return this.print(G, 0, P), !0;
+                                q = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).getString(I),
+                                X = new Uint32Array(q.length * A);
+                            let J = 0;
+                            for (let w = 0; w < q.length;) {
+                                const U = q.codePointAt(w) || 0;
+                                X[J++] = U, w += U > 65535 ? 2 : 1;
+                            }
+                            let P = J;
+                            for (let w = 1; w < A; ++w)
+                                X.copyWithin(P, 0, J), P += J;
+                            return this.print(X, 0, P), !0;
                         }
                         sendDeviceAttributesPrimary(C) {
                             return C.params[0] > 0 || (this._is("xterm") || this._is("rxvt-unicode") || this._is("screen") ? this._coreService.triggerDataEvent(a.C0.ESC + "[?1;2c") : this._is("linux") && this._coreService.triggerDataEvent(a.C0.ESC + "[?6c")), !0;
                         }
                         sendDeviceAttributesSecondary(C) {
                             return C.params[0] > 0 || (this._is("xterm") ? this._coreService.triggerDataEvent(a.C0.ESC + "[>0;276;0c") : this._is("rxvt-unicode") ? this._coreService.triggerDataEvent(a.C0.ESC + "[>85;95;0c") : this._is("linux") ? this._coreService.triggerDataEvent(C.params[0] + "c") : this._is("screen") && this._coreService.triggerDataEvent(a.C0.ESC + "[>83;40003;0c")), !0;
                         }
                         _is(C) {
                             return (this._optionsService.rawOptions.termName + "").indexOf(C) === 0;
                         }
                         setMode(C) {
-                            for (let D = 0; D < C.length; D++)
-                                switch (C.params[D]) {
+                            for (let x = 0; x < C.length; x++)
+                                switch (C.params[x]) {
                                     case 4:
                                         this._coreService.modes.insertMode = !0;
                                         break;
                                     case 20:
                                         this._optionsService.options.convertEol = !0;
                                 }
                             return !0;
                         }
                         setModePrivate(C) {
-                            for (let D = 0; D < C.length; D++)
-                                switch (C.params[D]) {
+                            for (let x = 0; x < C.length; x++)
+                                switch (C.params[x]) {
                                     case 1:
                                         this._coreService.decPrivateModes.applicationCursorKeys = !0;
                                         break;
                                     case 2:
                                         this._charsetService.setgCharset(0, d.DEFAULT_CHARSET), this._charsetService.setgCharset(1, d.DEFAULT_CHARSET), this._charsetService.setgCharset(2, d.DEFAULT_CHARSET), this._charsetService.setgCharset(3, d.DEFAULT_CHARSET);
                                         break;
                                     case 3:
@@ -6643,27 +6643,27 @@
                                         break;
                                     case 2004:
                                         this._coreService.decPrivateModes.bracketedPasteMode = !0;
                                 }
                             return !0;
                         }
                         resetMode(C) {
-                            for (let D = 0; D < C.length; D++)
-                                switch (C.params[D]) {
+                            for (let x = 0; x < C.length; x++)
+                                switch (C.params[x]) {
                                     case 4:
                                         this._coreService.modes.insertMode = !1;
                                         break;
                                     case 20:
                                         this._optionsService.options.convertEol = !1;
                                 }
                             return !0;
                         }
                         resetModePrivate(C) {
-                            for (let D = 0; D < C.length; D++)
-                                switch (C.params[D]) {
+                            for (let x = 0; x < C.length; x++)
+                                switch (C.params[x]) {
                                     case 1:
                                         this._coreService.decPrivateModes.applicationCursorKeys = !1;
                                         break;
                                     case 3:
                                         this._optionsService.rawOptions.windowOptions.setWinLines && (this._bufferService.resize(80, this._bufferService.rows), this._onRequestReset.fire());
                                         break;
                                     case 6:
@@ -6705,157 +6705,157 @@
                                         break;
                                     case 1048:
                                         this.restoreCursor();
                                         break;
                                     case 1049:
                                     case 47:
                                     case 1047:
-                                        this._bufferService.buffers.activateNormalBuffer(), C.params[D] === 1049 && this.restoreCursor(), this._coreService.isCursorInitialized = !0, this._onRequestRefreshRows.fire(0, this._bufferService.rows - 1), this._onRequestSyncScrollBar.fire();
+                                        this._bufferService.buffers.activateNormalBuffer(), C.params[x] === 1049 && this.restoreCursor(), this._coreService.isCursorInitialized = !0, this._onRequestRefreshRows.fire(0, this._bufferService.rows - 1), this._onRequestSyncScrollBar.fire();
                                         break;
                                     case 2004:
                                         this._coreService.decPrivateModes.bracketedPasteMode = !1;
                                 }
                             return !0;
                         }
-                        requestMode(C, D) {
-                            const B = this._coreService.decPrivateModes,
+                        requestMode(C, x) {
+                            const A = this._coreService.decPrivateModes,
                                 {
                                     activeProtocol: O,
                                     activeEncoding: I
                                 } = this._coreMouseService,
-                                z = this._coreService,
+                                q = this._coreService,
                                 {
-                                    buffers: G,
-                                    cols: X
+                                    buffers: X,
+                                    cols: J
                                 } = this._bufferService,
                                 {
                                     active: P,
                                     alt: w
-                                } = G,
-                                N = this._optionsService.rawOptions,
-                                F = (ie) => ie ? 1 : 2,
-                                V = C.params[0];
-                            return q = V, Z = D ? V === 2 ? 4 : V === 4 ? F(z.modes.insertMode) : V === 12 ? 3 : V === 20 ? F(N.convertEol) : 0 : V === 1 ? F(B.applicationCursorKeys) : V === 3 ? N.windowOptions.setWinLines ? X === 80 ? 2 : X === 132 ? 1 : 0 : 0 : V === 6 ? F(B.origin) : V === 7 ? F(B.wraparound) : V === 8 ? 3 : V === 9 ? F(O === "X10") : V === 12 ? F(N.cursorBlink) : V === 25 ? F(!z.isCursorHidden) : V === 45 ? F(B.reverseWraparound) : V === 66 ? F(B.applicationKeypad) : V === 67 ? 4 : V === 1e3 ? F(O === "VT200") : V === 1002 ? F(O === "DRAG") : V === 1003 ? F(O === "ANY") : V === 1004 ? F(B.sendFocus) : V === 1005 ? 4 : V === 1006 ? F(I === "SGR") : V === 1015 ? 4 : V === 1016 ? F(I === "SGR_PIXELS") : V === 1048 ? 1 : V === 47 || V === 1047 || V === 1049 ? F(P === w) : V === 2004 ? F(B.bracketedPasteMode) : 0, z.triggerDataEvent(`${a.C0.ESC}[${D ? "" : "?"}${q};${Z}$y`), !0;
-                            var q, Z;
+                                } = X,
+                                U = this._optionsService.rawOptions,
+                                F = (se) => se ? 1 : 2,
+                                G = C.params[0];
+                            return K = G, ee = x ? G === 2 ? 4 : G === 4 ? F(q.modes.insertMode) : G === 12 ? 3 : G === 20 ? F(U.convertEol) : 0 : G === 1 ? F(A.applicationCursorKeys) : G === 3 ? U.windowOptions.setWinLines ? J === 80 ? 2 : J === 132 ? 1 : 0 : 0 : G === 6 ? F(A.origin) : G === 7 ? F(A.wraparound) : G === 8 ? 3 : G === 9 ? F(O === "X10") : G === 12 ? F(U.cursorBlink) : G === 25 ? F(!q.isCursorHidden) : G === 45 ? F(A.reverseWraparound) : G === 66 ? F(A.applicationKeypad) : G === 67 ? 4 : G === 1e3 ? F(O === "VT200") : G === 1002 ? F(O === "DRAG") : G === 1003 ? F(O === "ANY") : G === 1004 ? F(A.sendFocus) : G === 1005 ? 4 : G === 1006 ? F(I === "SGR") : G === 1015 ? 4 : G === 1016 ? F(I === "SGR_PIXELS") : G === 1048 ? 1 : G === 47 || G === 1047 || G === 1049 ? F(P === w) : G === 2004 ? F(A.bracketedPasteMode) : 0, q.triggerDataEvent(`${a.C0.ESC}[${x ? "" : "?"}${K};${ee}$y`), !0;
+                            var K, ee;
                         }
-                        _updateAttrColor(C, D, B, O, I) {
-                            return D === 2 ? (C |= 50331648, C &= -16777216, C |= h.AttributeData.fromColorRGB([B, O, I])) : D === 5 && (C &= -50331904, C |= 33554432 | 255 & B), C;
+                        _updateAttrColor(C, x, A, O, I) {
+                            return x === 2 ? (C |= 50331648, C &= -16777216, C |= h.AttributeData.fromColorRGB([A, O, I])) : x === 5 && (C &= -50331904, C |= 33554432 | 255 & A), C;
                         }
-                        _extractColor(C, D, B) {
+                        _extractColor(C, x, A) {
                             const O = [0, 0, -1, 0, 0, 0];
                             let I = 0,
-                                z = 0;
+                                q = 0;
                             do {
-                                if (O[z + I] = C.params[D + z], C.hasSubParams(D + z)) {
-                                    const G = C.getSubParams(D + z);
-                                    let X = 0;
+                                if (O[q + I] = C.params[x + q], C.hasSubParams(x + q)) {
+                                    const X = C.getSubParams(x + q);
+                                    let J = 0;
                                     do
-                                        O[1] === 5 && (I = 1), O[z + X + 1 + I] = G[X];
-                                    while (++X < G.length && X + z + 1 + I < O.length);
+                                        O[1] === 5 && (I = 1), O[q + J + 1 + I] = X[J];
+                                    while (++J < X.length && J + q + 1 + I < O.length);
                                     break;
                                 }
-                                if (O[1] === 5 && z + I >= 2 || O[1] === 2 && z + I >= 5)
+                                if (O[1] === 5 && q + I >= 2 || O[1] === 2 && q + I >= 5)
                                     break;
                                 O[1] && (I = 1);
-                            } while (++z + D < C.length && z + I < O.length);
-                            for (let G = 2; G < O.length; ++G)
-                                O[G] === -1 && (O[G] = 0);
+                            } while (++q + x < C.length && q + I < O.length);
+                            for (let X = 2; X < O.length; ++X)
+                                O[X] === -1 && (O[X] = 0);
                             switch (O[0]) {
                                 case 38:
-                                    B.fg = this._updateAttrColor(B.fg, O[1], O[3], O[4], O[5]);
+                                    A.fg = this._updateAttrColor(A.fg, O[1], O[3], O[4], O[5]);
                                     break;
                                 case 48:
-                                    B.bg = this._updateAttrColor(B.bg, O[1], O[3], O[4], O[5]);
+                                    A.bg = this._updateAttrColor(A.bg, O[1], O[3], O[4], O[5]);
                                     break;
                                 case 58:
-                                    B.extended = B.extended.clone(), B.extended.underlineColor = this._updateAttrColor(B.extended.underlineColor, O[1], O[3], O[4], O[5]);
+                                    A.extended = A.extended.clone(), A.extended.underlineColor = this._updateAttrColor(A.extended.underlineColor, O[1], O[3], O[4], O[5]);
                             }
-                            return z;
+                            return q;
                         }
-                        _processUnderline(C, D) {
-                            D.extended = D.extended.clone(), (!~C || C > 5) && (C = 1), D.extended.underlineStyle = C, D.fg |= 268435456, C === 0 && (D.fg &= -268435457), D.updateExtended();
+                        _processUnderline(C, x) {
+                            x.extended = x.extended.clone(), (!~C || C > 5) && (C = 1), x.extended.underlineStyle = C, x.fg |= 268435456, C === 0 && (x.fg &= -268435457), x.updateExtended();
                         }
                         _processSGR0(C) {
                             C.fg = s.DEFAULT_ATTR_DATA.fg, C.bg = s.DEFAULT_ATTR_DATA.bg, C.extended = C.extended.clone(), C.extended.underlineStyle = 0, C.extended.underlineColor &= -67108864, C.updateExtended();
                         }
                         charAttributes(C) {
                             if (C.length === 1 && C.params[0] === 0)
                                 return this._processSGR0(this._curAttrData), !0;
-                            const D = C.length;
-                            let B;
+                            const x = C.length;
+                            let A;
                             const O = this._curAttrData;
-                            for (let I = 0; I < D; I++)
-                                B = C.params[I], B >= 30 && B <= 37 ? (O.fg &= -50331904, O.fg |= 16777216 | B - 30) : B >= 40 && B <= 47 ? (O.bg &= -50331904, O.bg |= 16777216 | B - 40) : B >= 90 && B <= 97 ? (O.fg &= -50331904, O.fg |= 16777224 | B - 90) : B >= 100 && B <= 107 ? (O.bg &= -50331904, O.bg |= 16777224 | B - 100) : B === 0 ? this._processSGR0(O) : B === 1 ? O.fg |= 134217728 : B === 3 ? O.bg |= 67108864 : B === 4 ? (O.fg |= 268435456, this._processUnderline(C.hasSubParams(I) ? C.getSubParams(I)[0] : 1, O)) : B === 5 ? O.fg |= 536870912 : B === 7 ? O.fg |= 67108864 : B === 8 ? O.fg |= 1073741824 : B === 9 ? O.fg |= 2147483648 : B === 2 ? O.bg |= 134217728 : B === 21 ? this._processUnderline(2, O) : B === 22 ? (O.fg &= -134217729, O.bg &= -134217729) : B === 23 ? O.bg &= -67108865 : B === 24 ? (O.fg &= -268435457, this._processUnderline(0, O)) : B === 25 ? O.fg &= -536870913 : B === 27 ? O.fg &= -67108865 : B === 28 ? O.fg &= -1073741825 : B === 29 ? O.fg &= 2147483647 : B === 39 ? (O.fg &= -67108864, O.fg |= 16777215 & s.DEFAULT_ATTR_DATA.fg) : B === 49 ? (O.bg &= -67108864, O.bg |= 16777215 & s.DEFAULT_ATTR_DATA.bg) : B === 38 || B === 48 || B === 58 ? I += this._extractColor(C, I, O) : B === 53 ? O.bg |= 1073741824 : B === 55 ? O.bg &= -1073741825 : B === 59 ? (O.extended = O.extended.clone(), O.extended.underlineColor = -1, O.updateExtended()) : B === 100 ? (O.fg &= -67108864, O.fg |= 16777215 & s.DEFAULT_ATTR_DATA.fg, O.bg &= -67108864, O.bg |= 16777215 & s.DEFAULT_ATTR_DATA.bg) : this._logService.debug("Unknown SGR attribute: %d.", B);
+                            for (let I = 0; I < x; I++)
+                                A = C.params[I], A >= 30 && A <= 37 ? (O.fg &= -50331904, O.fg |= 16777216 | A - 30) : A >= 40 && A <= 47 ? (O.bg &= -50331904, O.bg |= 16777216 | A - 40) : A >= 90 && A <= 97 ? (O.fg &= -50331904, O.fg |= 16777224 | A - 90) : A >= 100 && A <= 107 ? (O.bg &= -50331904, O.bg |= 16777224 | A - 100) : A === 0 ? this._processSGR0(O) : A === 1 ? O.fg |= 134217728 : A === 3 ? O.bg |= 67108864 : A === 4 ? (O.fg |= 268435456, this._processUnderline(C.hasSubParams(I) ? C.getSubParams(I)[0] : 1, O)) : A === 5 ? O.fg |= 536870912 : A === 7 ? O.fg |= 67108864 : A === 8 ? O.fg |= 1073741824 : A === 9 ? O.fg |= 2147483648 : A === 2 ? O.bg |= 134217728 : A === 21 ? this._processUnderline(2, O) : A === 22 ? (O.fg &= -134217729, O.bg &= -134217729) : A === 23 ? O.bg &= -67108865 : A === 24 ? (O.fg &= -268435457, this._processUnderline(0, O)) : A === 25 ? O.fg &= -536870913 : A === 27 ? O.fg &= -67108865 : A === 28 ? O.fg &= -1073741825 : A === 29 ? O.fg &= 2147483647 : A === 39 ? (O.fg &= -67108864, O.fg |= 16777215 & s.DEFAULT_ATTR_DATA.fg) : A === 49 ? (O.bg &= -67108864, O.bg |= 16777215 & s.DEFAULT_ATTR_DATA.bg) : A === 38 || A === 48 || A === 58 ? I += this._extractColor(C, I, O) : A === 53 ? O.bg |= 1073741824 : A === 55 ? O.bg &= -1073741825 : A === 59 ? (O.extended = O.extended.clone(), O.extended.underlineColor = -1, O.updateExtended()) : A === 100 ? (O.fg &= -67108864, O.fg |= 16777215 & s.DEFAULT_ATTR_DATA.fg, O.bg &= -67108864, O.bg |= 16777215 & s.DEFAULT_ATTR_DATA.bg) : this._logService.debug("Unknown SGR attribute: %d.", A);
                             return !0;
                         }
                         deviceStatus(C) {
                             switch (C.params[0]) {
                                 case 5:
                                     this._coreService.triggerDataEvent(`${a.C0.ESC}[0n`);
                                     break;
                                 case 6:
-                                    const D = this._activeBuffer.y + 1,
-                                        B = this._activeBuffer.x + 1;
-                                    this._coreService.triggerDataEvent(`${a.C0.ESC}[${D};${B}R`);
+                                    const x = this._activeBuffer.y + 1,
+                                        A = this._activeBuffer.x + 1;
+                                    this._coreService.triggerDataEvent(`${a.C0.ESC}[${x};${A}R`);
                             }
                             return !0;
                         }
                         deviceStatusPrivate(C) {
                             if (C.params[0] === 6) {
-                                const D = this._activeBuffer.y + 1,
-                                    B = this._activeBuffer.x + 1;
-                                this._coreService.triggerDataEvent(`${a.C0.ESC}[?${D};${B}R`);
+                                const x = this._activeBuffer.y + 1,
+                                    A = this._activeBuffer.x + 1;
+                                this._coreService.triggerDataEvent(`${a.C0.ESC}[?${x};${A}R`);
                             }
                             return !0;
                         }
                         softReset(C) {
                             return this._coreService.isCursorHidden = !1, this._onRequestSyncScrollBar.fire(), this._activeBuffer.scrollTop = 0, this._activeBuffer.scrollBottom = this._bufferService.rows - 1, this._curAttrData = s.DEFAULT_ATTR_DATA.clone(), this._coreService.reset(), this._charsetService.reset(), this._activeBuffer.savedX = 0, this._activeBuffer.savedY = this._activeBuffer.ybase, this._activeBuffer.savedCurAttrData.fg = this._curAttrData.fg, this._activeBuffer.savedCurAttrData.bg = this._curAttrData.bg, this._activeBuffer.savedCharset = this._charsetService.charset, this._coreService.decPrivateModes.origin = !1, !0;
                         }
                         setCursorStyle(C) {
-                            const D = C.params[0] || 1;
-                            switch (D) {
+                            const x = C.params[0] || 1;
+                            switch (x) {
                                 case 1:
                                 case 2:
                                     this._optionsService.options.cursorStyle = "block";
                                     break;
                                 case 3:
                                 case 4:
                                     this._optionsService.options.cursorStyle = "underline";
                                     break;
                                 case 5:
                                 case 6:
                                     this._optionsService.options.cursorStyle = "bar";
                             }
-                            const B = D % 2 == 1;
-                            return this._optionsService.options.cursorBlink = B, !0;
+                            const A = x % 2 == 1;
+                            return this._optionsService.options.cursorBlink = A, !0;
                         }
                         setScrollRegion(C) {
-                            const D = C.params[0] || 1;
-                            let B;
-                            return (C.length < 2 || (B = C.params[1]) > this._bufferService.rows || B === 0) && (B = this._bufferService.rows), B > D && (this._activeBuffer.scrollTop = D - 1, this._activeBuffer.scrollBottom = B - 1, this._setCursor(0, 0)), !0;
+                            const x = C.params[0] || 1;
+                            let A;
+                            return (C.length < 2 || (A = C.params[1]) > this._bufferService.rows || A === 0) && (A = this._bufferService.rows), A > x && (this._activeBuffer.scrollTop = x - 1, this._activeBuffer.scrollBottom = A - 1, this._setCursor(0, 0)), !0;
                         }
                         windowOptions(C) {
-                            if (!x(C.params[0], this._optionsService.rawOptions.windowOptions))
+                            if (!T(C.params[0], this._optionsService.rawOptions.windowOptions))
                                 return !0;
-                            const D = C.length > 1 ? C.params[1] : 0;
+                            const x = C.length > 1 ? C.params[1] : 0;
                             switch (C.params[0]) {
                                 case 14:
-                                    D !== 2 && this._onRequestWindowsOptionsReport.fire(L.GET_WIN_SIZE_PIXELS);
+                                    x !== 2 && this._onRequestWindowsOptionsReport.fire(L.GET_WIN_SIZE_PIXELS);
                                     break;
                                 case 16:
                                     this._onRequestWindowsOptionsReport.fire(L.GET_CELL_SIZE_PIXELS);
                                     break;
                                 case 18:
                                     this._bufferService && this._coreService.triggerDataEvent(`${a.C0.ESC}[8;${this._bufferService.rows};${this._bufferService.cols}t`);
                                     break;
                                 case 22:
-                                    D !== 0 && D !== 2 || (this._windowTitleStack.push(this._windowTitle), this._windowTitleStack.length > 10 && this._windowTitleStack.shift()), D !== 0 && D !== 1 || (this._iconNameStack.push(this._iconName), this._iconNameStack.length > 10 && this._iconNameStack.shift());
+                                    x !== 0 && x !== 2 || (this._windowTitleStack.push(this._windowTitle), this._windowTitleStack.length > 10 && this._windowTitleStack.shift()), x !== 0 && x !== 1 || (this._iconNameStack.push(this._iconName), this._iconNameStack.length > 10 && this._iconNameStack.shift());
                                     break;
                                 case 23:
-                                    D !== 0 && D !== 2 || this._windowTitleStack.length && this.setTitle(this._windowTitleStack.pop()), D !== 0 && D !== 1 || this._iconNameStack.length && this.setIconName(this._iconNameStack.pop());
+                                    x !== 0 && x !== 2 || this._windowTitleStack.length && this.setTitle(this._windowTitleStack.pop()), x !== 0 && x !== 1 || this._iconNameStack.length && this.setIconName(this._iconNameStack.pop());
                             }
                             return !0;
                         }
                         saveCursor(C) {
                             return this._activeBuffer.savedX = this._activeBuffer.x, this._activeBuffer.savedY = this._activeBuffer.ybase + this._activeBuffer.y, this._activeBuffer.savedCurAttrData.fg = this._curAttrData.fg, this._activeBuffer.savedCurAttrData.bg = this._curAttrData.bg, this._activeBuffer.savedCharset = this._charsetService.charset, !0;
                         }
                         restoreCursor(C) {
@@ -6864,69 +6864,69 @@
                         setTitle(C) {
                             return this._windowTitle = C, this._onTitleChange.fire(C), !0;
                         }
                         setIconName(C) {
                             return this._iconName = C, !0;
                         }
                         setOrReportIndexedColor(C) {
-                            const D = [],
-                                B = C.split(";");
-                            for (; B.length > 1;) {
-                                const O = B.shift(),
-                                    I = B.shift();
+                            const x = [],
+                                A = C.split(";");
+                            for (; A.length > 1;) {
+                                const O = A.shift(),
+                                    I = A.shift();
                                 if (/^\d+$/.exec(O)) {
-                                    const z = parseInt(O);
-                                    if (K(z))
+                                    const q = parseInt(O);
+                                    if (V(q))
                                         if (I === "?")
-                                            D.push({
+                                            x.push({
                                                 type: 0,
-                                                index: z
+                                                index: q
                                             });
                                         else {
-                                            const G = (0, b.parseColor)(I);
-                                            G && D.push({
+                                            const X = (0, b.parseColor)(I);
+                                            X && x.push({
                                                 type: 1,
-                                                index: z,
-                                                color: G
+                                                index: q,
+                                                color: X
                                             });
                                         }
                                 }
                             }
-                            return D.length && this._onColor.fire(D), !0;
+                            return x.length && this._onColor.fire(x), !0;
                         }
                         setHyperlink(C) {
-                            const D = C.split(";");
-                            return !(D.length < 2) && (D[1] ? this._createHyperlink(D[0], D[1]) : !D[0] && this._finishHyperlink());
+                            const x = C.split(";");
+                            return !(x.length < 2) && (x[1] ? this._createHyperlink(x[0], x[1]) : !x[0] && this._finishHyperlink());
                         }
-                        _createHyperlink(C, D) {
+                        _createHyperlink(C, x) {
                             this._getCurrentLinkId() && this._finishHyperlink();
-                            const B = C.split(":");
+                            const A = C.split(":");
                             let O;
-                            const I = B.findIndex((z) => z.startsWith("id="));
-                            return I !== -1 && (O = B[I].slice(3) || void 0), this._curAttrData.extended = this._curAttrData.extended.clone(), this._curAttrData.extended.urlId = this._oscLinkService.registerLink({
+                            const I = A.findIndex((q) => q.startsWith("id="));
+                            return I !== -1 && (O = A[I].slice(3) || void 0), this._curAttrData.extended = this._curAttrData.extended.clone(), this._curAttrData.extended.urlId = this._oscLinkService.registerLink({
                                 id: O,
-                                uri: D
+                                uri: x
                             }), this._curAttrData.updateExtended(), !0;
                         }
                         _finishHyperlink() {
                             return this._curAttrData.extended = this._curAttrData.extended.clone(), this._curAttrData.extended.urlId = 0, this._curAttrData.updateExtended(), !0;
                         }
-                        _setOrReportSpecialColor(C, D) {
-                            const B = C.split(";");
-                            for (let O = 0; O < B.length && !(D >= this._specialColors.length); ++O, ++D)
-                                if (B[O] === "?")
+                        _setOrReportSpecialColor(C, x) {
+                            const A = C.split(";");
+                            for (let O = 0; O < A.length && !(x >= this._specialColors.length); ++O, ++x)
+                                if (A[O] === "?")
                                     this._onColor.fire([{
                                         type: 0,
-                                        index: this._specialColors[D]
+                                        index: this._specialColors[x]
                                     }]);
                                 else {
-                                    const I = (0, b.parseColor)(B[O]);
+                                    const I = (0, b.parseColor)(A[O]);
                                     I && this._onColor.fire([{
                                         type: 1,
-                                        index: this._specialColors[D],
+                                        index: this._specialColors[x],
                                         color: I
                                     }]);
                                 }
                             return !0;
                         }
                         setOrReportFgColor(C) {
                             return this._setOrReportSpecialColor(C, 0);
@@ -6938,25 +6938,25 @@
                             return this._setOrReportSpecialColor(C, 2);
                         }
                         restoreIndexedColor(C) {
                             if (!C)
                                 return this._onColor.fire([{
                                     type: 2
                                 }]), !0;
-                            const D = [],
-                                B = C.split(";");
-                            for (let O = 0; O < B.length; ++O)
-                                if (/^\d+$/.exec(B[O])) {
-                                    const I = parseInt(B[O]);
-                                    K(I) && D.push({
+                            const x = [],
+                                A = C.split(";");
+                            for (let O = 0; O < A.length; ++O)
+                                if (/^\d+$/.exec(A[O])) {
+                                    const I = parseInt(A[O]);
+                                    V(I) && x.push({
                                         type: 2,
                                         index: I
                                     });
                                 }
-                            return D.length && this._onColor.fire(D), !0;
+                            return x.length && this._onColor.fire(x), !0;
                         }
                         restoreFgColor(C) {
                             return this._onColor.fire([{
                                 type: 2,
                                 index: 256
                             }]), !0;
                         }
@@ -6981,15 +6981,15 @@
                         keypadNumericMode() {
                             return this._logService.debug("Switching back to normal keypad."), this._coreService.decPrivateModes.applicationKeypad = !1, this._onRequestSyncScrollBar.fire(), !0;
                         }
                         selectDefaultCharset() {
                             return this._charsetService.setgLevel(0), this._charsetService.setgCharset(0, d.DEFAULT_CHARSET), !0;
                         }
                         selectCharset(C) {
-                            return C.length !== 2 ? (this.selectDefaultCharset(), !0) : (C[0] === "/" || this._charsetService.setgCharset(A[C[0]], d.CHARSETS[C[1]] || d.DEFAULT_CHARSET), !0);
+                            return C.length !== 2 ? (this.selectDefaultCharset(), !0) : (C[0] === "/" || this._charsetService.setgCharset(R[C[0]], d.CHARSETS[C[1]] || d.DEFAULT_CHARSET), !0);
                         }
                         index() {
                             return this._restrictCursor(), this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData())) : this._activeBuffer.y >= this._bufferService.rows && (this._activeBuffer.y = this._bufferService.rows - 1), this._restrictCursor(), !0;
                         }
                         tabSet() {
                             return this._activeBuffer.tabs[this._activeBuffer.x] = !0, !0;
                         }
@@ -7010,55 +7010,55 @@
                         _eraseAttrData() {
                             return this._eraseAttrDataInternal.bg &= -67108864, this._eraseAttrDataInternal.bg |= 67108863 & this._curAttrData.bg, this._eraseAttrDataInternal;
                         }
                         setgLevel(C) {
                             return this._charsetService.setgLevel(C), !0;
                         }
                         screenAlignmentPattern() {
-                            const C = new e.CellData();
+                            const C = new t.CellData();
                             C.content = 4194373, C.fg = this._curAttrData.fg, C.bg = this._curAttrData.bg, this._setCursor(0, 0);
-                            for (let D = 0; D < this._bufferService.rows; ++D) {
-                                const B = this._activeBuffer.ybase + this._activeBuffer.y + D,
-                                    O = this._activeBuffer.lines.get(B);
+                            for (let x = 0; x < this._bufferService.rows; ++x) {
+                                const A = this._activeBuffer.ybase + this._activeBuffer.y + x,
+                                    O = this._activeBuffer.lines.get(A);
                                 O && (O.fill(C), O.isWrapped = !1);
                             }
                             return this._dirtyRowTracker.markAllDirty(), this._setCursor(0, 0), !0;
                         }
-                        requestStatusString(C, D) {
-                            const B = this._bufferService.buffer,
+                        requestStatusString(C, x) {
+                            const A = this._bufferService.buffer,
                                 O = this._optionsService.rawOptions;
-                            return ((I) => (this._coreService.triggerDataEvent(`${a.C0.ESC}${I}${a.C0.ESC}\\`), !0))(C === '"q' ? `P1$r${this._curAttrData.isProtected() ? 1 : 0}"q` : C === '"p' ? 'P1$r61;1"p' : C === "r" ? `P1$r${B.scrollTop + 1};${B.scrollBottom + 1}r` : C === "m" ? "P1$r0m" : C === " q" ? `P1$r${{ block: 2, underline: 4, bar: 6 }[O.cursorStyle] - (O.cursorBlink ? 1 : 0)} q` : "P0$r");
+                            return ((I) => (this._coreService.triggerDataEvent(`${a.C0.ESC}${I}${a.C0.ESC}\\`), !0))(C === '"q' ? `P1$r${this._curAttrData.isProtected() ? 1 : 0}"q` : C === '"p' ? 'P1$r61;1"p' : C === "r" ? `P1$r${A.scrollTop + 1};${A.scrollBottom + 1}r` : C === "m" ? "P1$r0m" : C === " q" ? `P1$r${{ block: 2, underline: 4, bar: 6 }[O.cursorStyle] - (O.cursorBlink ? 1 : 0)} q` : "P0$r");
                         }
-                        markRangeDirty(C, D) {
-                            this._dirtyRowTracker.markRangeDirty(C, D);
+                        markRangeDirty(C, x) {
+                            this._dirtyRowTracker.markRangeDirty(C, x);
                         }
                     }
                     i.InputHandler = W;
-                    let U = class {
-                        constructor(j) {
-                            this._bufferService = j, this.clearRange();
+                    let j = class {
+                        constructor(z) {
+                            this._bufferService = z, this.clearRange();
                         }
                         clearRange() {
                             this.start = this._bufferService.buffer.y, this.end = this._bufferService.buffer.y;
                         }
-                        markDirty(j) {
-                            j < this.start ? this.start = j : j > this.end && (this.end = j);
+                        markDirty(z) {
+                            z < this.start ? this.start = z : z > this.end && (this.end = z);
                         }
-                        markRangeDirty(j, C) {
-                            j > C && (H = j, j = C, C = H), j < this.start && (this.start = j), C > this.end && (this.end = C);
+                        markRangeDirty(z, C) {
+                            z > C && (H = z, z = C, C = H), z < this.start && (this.start = z), C > this.end && (this.end = C);
                         }
                         markAllDirty() {
                             this.markRangeDirty(0, this._bufferService.rows - 1);
                         }
                     };
 
-                    function K(j) {
-                        return 0 <= j && j < 256;
+                    function V(z) {
+                        return 0 <= z && z < 256;
                     }
-                    U = o([c(0, v.IBufferService)], U);
+                    j = o([c(0, g.IBufferService)], j);
                 },
                 844: (k, i) => {
                     function n(o) {
                         for (const c of o)
                             c.dispose();
                         o.length = 0;
                     }
@@ -7127,20 +7127,20 @@
                             this._data = {};
                         }
                     }
                     i.TwoKeyMap = n, i.FourKeyMap = class {
                         constructor() {
                             this._data = new n();
                         }
-                        set(o, c, a, d, f) {
-                            this._data.get(o, c) || this._data.set(o, c, new n()), this._data.get(o, c).set(a, d, f);
+                        set(o, c, a, d, v) {
+                            this._data.get(o, c) || this._data.set(o, c, new n()), this._data.get(o, c).set(a, d, v);
                         }
                         get(o, c, a, d) {
-                            var f;
-                            return (f = this._data.get(o, c)) == null ? void 0 : f.get(a, d);
+                            var v;
+                            return (v = this._data.get(o, c)) == null ? void 0 : v.get(a, d);
                         }
                         clear() {
                             this._data.clear();
                         }
                     };
                 },
                 6114: (k, i) => {
@@ -7199,19 +7199,19 @@
                             return [...this._array].values();
                         }
                         _search(o) {
                             let c = 0,
                                 a = this._array.length - 1;
                             for (; a >= c;) {
                                 let d = c + a >> 1;
-                                const f = this._getKey(this._array[d]);
-                                if (f > o)
+                                const v = this._getKey(this._array[d]);
+                                if (v > o)
                                     a = d - 1;
                                 else {
-                                    if (!(f < o)) {
+                                    if (!(v < o)) {
                                         for (; d > 0 && this._getKey(this._array[d - 1]) === o;)
                                             d--;
                                         return d;
                                     }
                                     c = d + 1;
                                 }
                             }
@@ -7224,53 +7224,53 @@
                         value: !0
                     }), i.DebouncedIdleTask = i.IdleTaskQueue = i.PriorityTaskQueue = void 0;
                     const o = n(6114);
                     class c {
                         constructor() {
                             this._tasks = [], this._i = 0;
                         }
-                        enqueue(f) {
-                            this._tasks.push(f), this._start();
+                        enqueue(v) {
+                            this._tasks.push(v), this._start();
                         }
                         flush() {
                             for (; this._i < this._tasks.length;)
                                 this._tasks[this._i]() || this._i++;
                             this.clear();
                         }
                         clear() {
                             this._idleCallback && (this._cancelCallback(this._idleCallback), this._idleCallback = void 0), this._i = 0, this._tasks.length = 0;
                         }
                         _start() {
                             this._idleCallback || (this._idleCallback = this._requestCallback(this._process.bind(this)));
                         }
-                        _process(f) {
+                        _process(v) {
                             this._idleCallback = void 0;
-                            let g = 0,
+                            let m = 0,
                                 l = 0,
-                                s = f.timeRemaining(),
+                                s = v.timeRemaining(),
                                 r = 0;
                             for (; this._i < this._tasks.length;) {
-                                if (g = Date.now(), this._tasks[this._i]() || this._i++, g = Math.max(1, Date.now() - g), l = Math.max(g, l), r = f.timeRemaining(), 1.5 * l > r)
-                                    return s - g < -20 && console.warn(`task queue exceeded allotted deadline by ${Math.abs(Math.round(s - g))}ms`), void this._start();
+                                if (m = Date.now(), this._tasks[this._i]() || this._i++, m = Math.max(1, Date.now() - m), l = Math.max(m, l), r = v.timeRemaining(), 1.5 * l > r)
+                                    return s - m < -20 && console.warn(`task queue exceeded allotted deadline by ${Math.abs(Math.round(s - m))}ms`), void this._start();
                                 s = r;
                             }
                             this.clear();
                         }
                     }
                     class a extends c {
-                        _requestCallback(f) {
-                            return setTimeout(() => f(this._createDeadline(16)));
+                        _requestCallback(v) {
+                            return setTimeout(() => v(this._createDeadline(16)));
                         }
-                        _cancelCallback(f) {
-                            clearTimeout(f);
+                        _cancelCallback(v) {
+                            clearTimeout(v);
                         }
-                        _createDeadline(f) {
-                            const g = Date.now() + f;
+                        _createDeadline(v) {
+                            const m = Date.now() + v;
                             return {
-                                timeRemaining: () => Math.max(0, g - Date.now())
+                                timeRemaining: () => Math.max(0, m - Date.now())
                             };
                         }
                     }
                     i.PriorityTaskQueue = a, i.IdleTaskQueue = !o.isNode && "requestIdleCallback" in window ? class extends c {
                         _requestCallback(d) {
                             return requestIdleCallback(d);
                         }
@@ -7293,16 +7293,16 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.updateWindowsModeWrappedState = void 0;
                     const o = n(643);
                     i.updateWindowsModeWrappedState = function(c) {
                         const a = c.buffer.lines.get(c.buffer.ybase + c.buffer.y - 1),
                             d = a == null ? void 0 : a.get(c.cols - 1),
-                            f = c.buffer.lines.get(c.buffer.ybase + c.buffer.y);
-                        f && d && (f.isWrapped = d[o.CHAR_DATA_CODE_INDEX] !== o.NULL_CELL_CODE && d[o.CHAR_DATA_CODE_INDEX] !== o.WHITESPACE_CELL_CODE);
+                            v = c.buffer.lines.get(c.buffer.ybase + c.buffer.y);
+                        v && d && (v.isWrapped = d[o.CHAR_DATA_CODE_INDEX] !== o.NULL_CELL_CODE && d[o.CHAR_DATA_CODE_INDEX] !== o.WHITESPACE_CELL_CODE);
                     };
                 },
                 3734: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.ExtendedAttrs = i.AttributeData = void 0;
                     class n {
@@ -7485,269 +7485,269 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.Buffer = i.MAX_BUFFER_SIZE = void 0;
                     const o = n(6349),
                         c = n(7226),
                         a = n(3734),
                         d = n(8437),
-                        f = n(4634),
-                        g = n(511),
+                        v = n(4634),
+                        m = n(511),
                         l = n(643),
                         s = n(4863),
                         r = n(7116);
                     i.MAX_BUFFER_SIZE = 4294967295, i.Buffer = class {
-                        constructor(t, e, h) {
-                            this._hasScrollback = t, this._optionsService = e, this._bufferService = h, this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.tabs = {}, this.savedY = 0, this.savedX = 0, this.savedCurAttrData = d.DEFAULT_ATTR_DATA.clone(), this.savedCharset = r.DEFAULT_CHARSET, this.markers = [], this._nullCell = g.CellData.fromCharData([0, l.NULL_CELL_CHAR, l.NULL_CELL_WIDTH, l.NULL_CELL_CODE]), this._whitespaceCell = g.CellData.fromCharData([0, l.WHITESPACE_CELL_CHAR, l.WHITESPACE_CELL_WIDTH, l.WHITESPACE_CELL_CODE]), this._isClearing = !1, this._memoryCleanupQueue = new c.IdleTaskQueue(), this._memoryCleanupPosition = 0, this._cols = this._bufferService.cols, this._rows = this._bufferService.rows, this.lines = new o.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
+                        constructor(e, t, h) {
+                            this._hasScrollback = e, this._optionsService = t, this._bufferService = h, this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.tabs = {}, this.savedY = 0, this.savedX = 0, this.savedCurAttrData = d.DEFAULT_ATTR_DATA.clone(), this.savedCharset = r.DEFAULT_CHARSET, this.markers = [], this._nullCell = m.CellData.fromCharData([0, l.NULL_CELL_CHAR, l.NULL_CELL_WIDTH, l.NULL_CELL_CODE]), this._whitespaceCell = m.CellData.fromCharData([0, l.WHITESPACE_CELL_CHAR, l.WHITESPACE_CELL_WIDTH, l.WHITESPACE_CELL_CODE]), this._isClearing = !1, this._memoryCleanupQueue = new c.IdleTaskQueue(), this._memoryCleanupPosition = 0, this._cols = this._bufferService.cols, this._rows = this._bufferService.rows, this.lines = new o.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
                         }
-                        getNullCell(t) {
-                            return t ? (this._nullCell.fg = t.fg, this._nullCell.bg = t.bg, this._nullCell.extended = t.extended) : (this._nullCell.fg = 0, this._nullCell.bg = 0, this._nullCell.extended = new a.ExtendedAttrs()), this._nullCell;
+                        getNullCell(e) {
+                            return e ? (this._nullCell.fg = e.fg, this._nullCell.bg = e.bg, this._nullCell.extended = e.extended) : (this._nullCell.fg = 0, this._nullCell.bg = 0, this._nullCell.extended = new a.ExtendedAttrs()), this._nullCell;
                         }
-                        getWhitespaceCell(t) {
-                            return t ? (this._whitespaceCell.fg = t.fg, this._whitespaceCell.bg = t.bg, this._whitespaceCell.extended = t.extended) : (this._whitespaceCell.fg = 0, this._whitespaceCell.bg = 0, this._whitespaceCell.extended = new a.ExtendedAttrs()), this._whitespaceCell;
+                        getWhitespaceCell(e) {
+                            return e ? (this._whitespaceCell.fg = e.fg, this._whitespaceCell.bg = e.bg, this._whitespaceCell.extended = e.extended) : (this._whitespaceCell.fg = 0, this._whitespaceCell.bg = 0, this._whitespaceCell.extended = new a.ExtendedAttrs()), this._whitespaceCell;
                         }
-                        getBlankLine(t, e) {
-                            return new d.BufferLine(this._bufferService.cols, this.getNullCell(t), e);
+                        getBlankLine(e, t) {
+                            return new d.BufferLine(this._bufferService.cols, this.getNullCell(e), t);
                         }
                         get hasScrollback() {
                             return this._hasScrollback && this.lines.maxLength > this._rows;
                         }
                         get isCursorInViewport() {
-                            const t = this.ybase + this.y - this.ydisp;
-                            return t >= 0 && t < this._rows;
+                            const e = this.ybase + this.y - this.ydisp;
+                            return e >= 0 && e < this._rows;
                         }
-                        _getCorrectBufferLength(t) {
+                        _getCorrectBufferLength(e) {
                             if (!this._hasScrollback)
-                                return t;
-                            const e = t + this._optionsService.rawOptions.scrollback;
-                            return e > i.MAX_BUFFER_SIZE ? i.MAX_BUFFER_SIZE : e;
+                                return e;
+                            const t = e + this._optionsService.rawOptions.scrollback;
+                            return t > i.MAX_BUFFER_SIZE ? i.MAX_BUFFER_SIZE : t;
                         }
-                        fillViewportRows(t) {
+                        fillViewportRows(e) {
                             if (this.lines.length === 0) {
-                                t === void 0 && (t = d.DEFAULT_ATTR_DATA);
-                                let e = this._rows;
-                                for (; e--;)
-                                    this.lines.push(this.getBlankLine(t));
+                                e === void 0 && (e = d.DEFAULT_ATTR_DATA);
+                                let t = this._rows;
+                                for (; t--;)
+                                    this.lines.push(this.getBlankLine(e));
                             }
                         }
                         clear() {
                             this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.lines = new o.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
                         }
-                        resize(t, e) {
+                        resize(e, t) {
                             const h = this.getNullCell(d.DEFAULT_ATTR_DATA);
-                            let v = 0;
-                            const u = this._getCorrectBufferLength(e);
+                            let g = 0;
+                            const u = this._getCorrectBufferLength(t);
                             if (u > this.lines.maxLength && (this.lines.maxLength = u), this.lines.length > 0) {
-                                if (this._cols < t)
+                                if (this._cols < e)
                                     for (let _ = 0; _ < this.lines.length; _++)
-                                        v += +this.lines.get(_).resize(t, h);
-                                let p = 0;
-                                if (this._rows < e)
-                                    for (let _ = this._rows; _ < e; _++)
-                                        this.lines.length < e + this.ybase && (this._optionsService.rawOptions.windowsMode || this._optionsService.rawOptions.windowsPty.backend !== void 0 || this._optionsService.rawOptions.windowsPty.buildNumber !== void 0 ? this.lines.push(new d.BufferLine(t, h)) : this.ybase > 0 && this.lines.length <= this.ybase + this.y + p + 1 ? (this.ybase--, p++, this.ydisp > 0 && this.ydisp--) : this.lines.push(new d.BufferLine(t, h)));
+                                        g += +this.lines.get(_).resize(e, h);
+                                let S = 0;
+                                if (this._rows < t)
+                                    for (let _ = this._rows; _ < t; _++)
+                                        this.lines.length < t + this.ybase && (this._optionsService.rawOptions.windowsMode || this._optionsService.rawOptions.windowsPty.backend !== void 0 || this._optionsService.rawOptions.windowsPty.buildNumber !== void 0 ? this.lines.push(new d.BufferLine(e, h)) : this.ybase > 0 && this.lines.length <= this.ybase + this.y + S + 1 ? (this.ybase--, S++, this.ydisp > 0 && this.ydisp--) : this.lines.push(new d.BufferLine(e, h)));
                                 else
-                                    for (let _ = this._rows; _ > e; _--)
-                                        this.lines.length > e + this.ybase && (this.lines.length > this.ybase + this.y + 1 ? this.lines.pop() : (this.ybase++, this.ydisp++));
+                                    for (let _ = this._rows; _ > t; _--)
+                                        this.lines.length > t + this.ybase && (this.lines.length > this.ybase + this.y + 1 ? this.lines.pop() : (this.ybase++, this.ydisp++));
                                 if (u < this.lines.maxLength) {
                                     const _ = this.lines.length - u;
                                     _ > 0 && (this.lines.trimStart(_), this.ybase = Math.max(this.ybase - _, 0), this.ydisp = Math.max(this.ydisp - _, 0), this.savedY = Math.max(this.savedY - _, 0)), this.lines.maxLength = u;
                                 }
-                                this.x = Math.min(this.x, t - 1), this.y = Math.min(this.y, e - 1), p && (this.y += p), this.savedX = Math.min(this.savedX, t - 1), this.scrollTop = 0;
+                                this.x = Math.min(this.x, e - 1), this.y = Math.min(this.y, t - 1), S && (this.y += S), this.savedX = Math.min(this.savedX, e - 1), this.scrollTop = 0;
                             }
-                            if (this.scrollBottom = e - 1, this._isReflowEnabled && (this._reflow(t, e), this._cols > t))
-                                for (let p = 0; p < this.lines.length; p++)
-                                    v += +this.lines.get(p).resize(t, h);
-                            this._cols = t, this._rows = e, this._memoryCleanupQueue.clear(), v > 0.1 * this.lines.length && (this._memoryCleanupPosition = 0, this._memoryCleanupQueue.enqueue(() => this._batchedMemoryCleanup()));
+                            if (this.scrollBottom = t - 1, this._isReflowEnabled && (this._reflow(e, t), this._cols > e))
+                                for (let S = 0; S < this.lines.length; S++)
+                                    g += +this.lines.get(S).resize(e, h);
+                            this._cols = e, this._rows = t, this._memoryCleanupQueue.clear(), g > 0.1 * this.lines.length && (this._memoryCleanupPosition = 0, this._memoryCleanupQueue.enqueue(() => this._batchedMemoryCleanup()));
                         }
                         _batchedMemoryCleanup() {
-                            let t = !0;
-                            this._memoryCleanupPosition >= this.lines.length && (this._memoryCleanupPosition = 0, t = !1);
-                            let e = 0;
+                            let e = !0;
+                            this._memoryCleanupPosition >= this.lines.length && (this._memoryCleanupPosition = 0, e = !1);
+                            let t = 0;
                             for (; this._memoryCleanupPosition < this.lines.length;)
-                                if (e += this.lines.get(this._memoryCleanupPosition++).cleanupMemory(), e > 100)
+                                if (t += this.lines.get(this._memoryCleanupPosition++).cleanupMemory(), t > 100)
                                     return !0;
-                            return t;
+                            return e;
                         }
                         get _isReflowEnabled() {
-                            const t = this._optionsService.rawOptions.windowsPty;
-                            return t && t.buildNumber ? this._hasScrollback && t.backend === "conpty" && t.buildNumber >= 21376 : this._hasScrollback && !this._optionsService.rawOptions.windowsMode;
+                            const e = this._optionsService.rawOptions.windowsPty;
+                            return e && e.buildNumber ? this._hasScrollback && e.backend === "conpty" && e.buildNumber >= 21376 : this._hasScrollback && !this._optionsService.rawOptions.windowsMode;
                         }
-                        _reflow(t, e) {
-                            this._cols !== t && (t > this._cols ? this._reflowLarger(t, e) : this._reflowSmaller(t, e));
+                        _reflow(e, t) {
+                            this._cols !== e && (e > this._cols ? this._reflowLarger(e, t) : this._reflowSmaller(e, t));
                         }
-                        _reflowLarger(t, e) {
-                            const h = (0, f.reflowLargerGetLinesToRemove)(this.lines, this._cols, t, this.ybase + this.y, this.getNullCell(d.DEFAULT_ATTR_DATA));
+                        _reflowLarger(e, t) {
+                            const h = (0, v.reflowLargerGetLinesToRemove)(this.lines, this._cols, e, this.ybase + this.y, this.getNullCell(d.DEFAULT_ATTR_DATA));
                             if (h.length > 0) {
-                                const v = (0, f.reflowLargerCreateNewLayout)(this.lines, h);
-                                (0, f.reflowLargerApplyNewLayout)(this.lines, v.layout), this._reflowLargerAdjustViewport(t, e, v.countRemoved);
+                                const g = (0, v.reflowLargerCreateNewLayout)(this.lines, h);
+                                (0, v.reflowLargerApplyNewLayout)(this.lines, g.layout), this._reflowLargerAdjustViewport(e, t, g.countRemoved);
                             }
                         }
-                        _reflowLargerAdjustViewport(t, e, h) {
-                            const v = this.getNullCell(d.DEFAULT_ATTR_DATA);
+                        _reflowLargerAdjustViewport(e, t, h) {
+                            const g = this.getNullCell(d.DEFAULT_ATTR_DATA);
                             let u = h;
                             for (; u-- > 0;)
-                                this.ybase === 0 ? (this.y > 0 && this.y--, this.lines.length < e && this.lines.push(new d.BufferLine(t, v))) : (this.ydisp === this.ybase && this.ydisp--, this.ybase--);
+                                this.ybase === 0 ? (this.y > 0 && this.y--, this.lines.length < t && this.lines.push(new d.BufferLine(e, g))) : (this.ydisp === this.ybase && this.ydisp--, this.ybase--);
                             this.savedY = Math.max(this.savedY - h, 0);
                         }
-                        _reflowSmaller(t, e) {
+                        _reflowSmaller(e, t) {
                             const h = this.getNullCell(d.DEFAULT_ATTR_DATA),
-                                v = [];
+                                g = [];
                             let u = 0;
-                            for (let p = this.lines.length - 1; p >= 0; p--) {
-                                let _ = this.lines.get(p);
-                                if (!_ || !_.isWrapped && _.getTrimmedLength() <= t)
+                            for (let S = this.lines.length - 1; S >= 0; S--) {
+                                let _ = this.lines.get(S);
+                                if (!_ || !_.isWrapped && _.getTrimmedLength() <= e)
                                     continue;
                                 const b = [_];
-                                for (; _.isWrapped && p > 0;)
-                                    _ = this.lines.get(--p), b.unshift(_);
-                                const A = this.ybase + this.y;
-                                if (A >= p && A < p + b.length)
+                                for (; _.isWrapped && S > 0;)
+                                    _ = this.lines.get(--S), b.unshift(_);
+                                const R = this.ybase + this.y;
+                                if (R >= S && R < S + b.length)
                                     continue;
-                                const T = b[b.length - 1].getTrimmedLength(),
-                                    x = (0, f.reflowSmallerGetNewLineLengths)(b, this._cols, t),
-                                    L = x.length - b.length;
+                                const B = b[b.length - 1].getTrimmedLength(),
+                                    T = (0, v.reflowSmallerGetNewLineLengths)(b, this._cols, e),
+                                    L = T.length - b.length;
                                 let H;
                                 H = this.ybase === 0 && this.y !== this.lines.length - 1 ? Math.max(0, this.y - this.lines.maxLength + L) : Math.max(0, this.lines.length - this.lines.maxLength + L);
                                 const W = [];
-                                for (let B = 0; B < L; B++) {
+                                for (let A = 0; A < L; A++) {
                                     const O = this.getBlankLine(d.DEFAULT_ATTR_DATA, !0);
                                     W.push(O);
                                 }
-                                W.length > 0 && (v.push({
-                                    start: p + b.length + u,
+                                W.length > 0 && (g.push({
+                                    start: S + b.length + u,
                                     newLines: W
                                 }), u += W.length), b.push(...W);
-                                let U = x.length - 1,
-                                    K = x[U];
-                                K === 0 && (U--, K = x[U]);
-                                let j = b.length - L - 1,
-                                    C = T;
-                                for (; j >= 0;) {
-                                    const B = Math.min(C, K);
-                                    if (b[U] === void 0)
-                                        break;
-                                    if (b[U].copyCellsFrom(b[j], C - B, K - B, B, !0), K -= B, K === 0 && (U--, K = x[U]), C -= B, C === 0) {
-                                        j--;
-                                        const O = Math.max(j, 0);
-                                        C = (0, f.getWrappedLineTrimmedLength)(b, O, this._cols);
+                                let j = T.length - 1,
+                                    V = T[j];
+                                V === 0 && (j--, V = T[j]);
+                                let z = b.length - L - 1,
+                                    C = B;
+                                for (; z >= 0;) {
+                                    const A = Math.min(C, V);
+                                    if (b[j] === void 0)
+                                        break;
+                                    if (b[j].copyCellsFrom(b[z], C - A, V - A, A, !0), V -= A, V === 0 && (j--, V = T[j]), C -= A, C === 0) {
+                                        z--;
+                                        const O = Math.max(z, 0);
+                                        C = (0, v.getWrappedLineTrimmedLength)(b, O, this._cols);
                                     }
                                 }
-                                for (let B = 0; B < b.length; B++)
-                                    x[B] < t && b[B].setCell(x[B], h);
-                                let D = L - H;
-                                for (; D-- > 0;)
-                                    this.ybase === 0 ? this.y < e - 1 ? (this.y++, this.lines.pop()) : (this.ybase++, this.ydisp++) : this.ybase < Math.min(this.lines.maxLength, this.lines.length + u) - e && (this.ybase === this.ydisp && this.ydisp++, this.ybase++);
-                                this.savedY = Math.min(this.savedY + L, this.ybase + e - 1);
+                                for (let A = 0; A < b.length; A++)
+                                    T[A] < e && b[A].setCell(T[A], h);
+                                let x = L - H;
+                                for (; x-- > 0;)
+                                    this.ybase === 0 ? this.y < t - 1 ? (this.y++, this.lines.pop()) : (this.ybase++, this.ydisp++) : this.ybase < Math.min(this.lines.maxLength, this.lines.length + u) - t && (this.ybase === this.ydisp && this.ydisp++, this.ybase++);
+                                this.savedY = Math.min(this.savedY + L, this.ybase + t - 1);
                             }
-                            if (v.length > 0) {
-                                const p = [],
+                            if (g.length > 0) {
+                                const S = [],
                                     _ = [];
-                                for (let U = 0; U < this.lines.length; U++)
-                                    _.push(this.lines.get(U));
+                                for (let j = 0; j < this.lines.length; j++)
+                                    _.push(this.lines.get(j));
                                 const b = this.lines.length;
-                                let A = b - 1,
-                                    T = 0,
-                                    x = v[T];
+                                let R = b - 1,
+                                    B = 0,
+                                    T = g[B];
                                 this.lines.length = Math.min(this.lines.maxLength, this.lines.length + u);
                                 let L = 0;
-                                for (let U = Math.min(this.lines.maxLength - 1, b + u - 1); U >= 0; U--)
-                                    if (x && x.start > A + L) {
-                                        for (let K = x.newLines.length - 1; K >= 0; K--)
-                                            this.lines.set(U--, x.newLines[K]);
-                                        U++, p.push({
-                                            index: A + 1,
-                                            amount: x.newLines.length
-                                        }), L += x.newLines.length, x = v[++T];
+                                for (let j = Math.min(this.lines.maxLength - 1, b + u - 1); j >= 0; j--)
+                                    if (T && T.start > R + L) {
+                                        for (let V = T.newLines.length - 1; V >= 0; V--)
+                                            this.lines.set(j--, T.newLines[V]);
+                                        j++, S.push({
+                                            index: R + 1,
+                                            amount: T.newLines.length
+                                        }), L += T.newLines.length, T = g[++B];
                                     } else
-                                        this.lines.set(U, _[A--]);
+                                        this.lines.set(j, _[R--]);
                                 let H = 0;
-                                for (let U = p.length - 1; U >= 0; U--)
-                                    p[U].index += H, this.lines.onInsertEmitter.fire(p[U]), H += p[U].amount;
+                                for (let j = S.length - 1; j >= 0; j--)
+                                    S[j].index += H, this.lines.onInsertEmitter.fire(S[j]), H += S[j].amount;
                                 const W = Math.max(0, b + u - this.lines.maxLength);
                                 W > 0 && this.lines.onTrimEmitter.fire(W);
                             }
                         }
-                        translateBufferLineToString(t, e, h = 0, v) {
-                            const u = this.lines.get(t);
-                            return u ? u.translateToString(e, h, v) : "";
-                        }
-                        getWrappedRangeForLine(t) {
-                            let e = t,
-                                h = t;
-                            for (; e > 0 && this.lines.get(e).isWrapped;)
-                                e--;
+                        translateBufferLineToString(e, t, h = 0, g) {
+                            const u = this.lines.get(e);
+                            return u ? u.translateToString(t, h, g) : "";
+                        }
+                        getWrappedRangeForLine(e) {
+                            let t = e,
+                                h = e;
+                            for (; t > 0 && this.lines.get(t).isWrapped;)
+                                t--;
                             for (; h + 1 < this.lines.length && this.lines.get(h + 1).isWrapped;)
                                 h++;
                             return {
-                                first: e,
+                                first: t,
                                 last: h
                             };
                         }
-                        setupTabStops(t) {
-                            for (t != null ? this.tabs[t] || (t = this.prevStop(t)) : (this.tabs = {}, t = 0); t < this._cols; t += this._optionsService.rawOptions.tabStopWidth)
-                                this.tabs[t] = !0;
+                        setupTabStops(e) {
+                            for (e != null ? this.tabs[e] || (e = this.prevStop(e)) : (this.tabs = {}, e = 0); e < this._cols; e += this._optionsService.rawOptions.tabStopWidth)
+                                this.tabs[e] = !0;
                         }
-                        prevStop(t) {
-                            for (t == null && (t = this.x); !this.tabs[--t] && t > 0;)
+                        prevStop(e) {
+                            for (e == null && (e = this.x); !this.tabs[--e] && e > 0;)
                             ;
-                            return t >= this._cols ? this._cols - 1 : t < 0 ? 0 : t;
+                            return e >= this._cols ? this._cols - 1 : e < 0 ? 0 : e;
                         }
-                        nextStop(t) {
-                            for (t == null && (t = this.x); !this.tabs[++t] && t < this._cols;)
+                        nextStop(e) {
+                            for (e == null && (e = this.x); !this.tabs[++e] && e < this._cols;)
                             ;
-                            return t >= this._cols ? this._cols - 1 : t < 0 ? 0 : t;
+                            return e >= this._cols ? this._cols - 1 : e < 0 ? 0 : e;
                         }
-                        clearMarkers(t) {
+                        clearMarkers(e) {
                             this._isClearing = !0;
-                            for (let e = 0; e < this.markers.length; e++)
-                                this.markers[e].line === t && (this.markers[e].dispose(), this.markers.splice(e--, 1));
+                            for (let t = 0; t < this.markers.length; t++)
+                                this.markers[t].line === e && (this.markers[t].dispose(), this.markers.splice(t--, 1));
                             this._isClearing = !1;
                         }
                         clearAllMarkers() {
                             this._isClearing = !0;
-                            for (let t = 0; t < this.markers.length; t++)
-                                this.markers[t].dispose(), this.markers.splice(t--, 1);
+                            for (let e = 0; e < this.markers.length; e++)
+                                this.markers[e].dispose(), this.markers.splice(e--, 1);
                             this._isClearing = !1;
                         }
-                        addMarker(t) {
-                            const e = new s.Marker(t);
-                            return this.markers.push(e), e.register(this.lines.onTrim((h) => {
-                                e.line -= h, e.line < 0 && e.dispose();
-                            })), e.register(this.lines.onInsert((h) => {
-                                e.line >= h.index && (e.line += h.amount);
-                            })), e.register(this.lines.onDelete((h) => {
-                                e.line >= h.index && e.line < h.index + h.amount && e.dispose(), e.line > h.index && (e.line -= h.amount);
-                            })), e.register(e.onDispose(() => this._removeMarker(e))), e;
+                        addMarker(e) {
+                            const t = new s.Marker(e);
+                            return this.markers.push(t), t.register(this.lines.onTrim((h) => {
+                                t.line -= h, t.line < 0 && t.dispose();
+                            })), t.register(this.lines.onInsert((h) => {
+                                t.line >= h.index && (t.line += h.amount);
+                            })), t.register(this.lines.onDelete((h) => {
+                                t.line >= h.index && t.line < h.index + h.amount && t.dispose(), t.line > h.index && (t.line -= h.amount);
+                            })), t.register(t.onDispose(() => this._removeMarker(t))), t;
                         }
-                        _removeMarker(t) {
-                            this._isClearing || this.markers.splice(this.markers.indexOf(t), 1);
+                        _removeMarker(e) {
+                            this._isClearing || this.markers.splice(this.markers.indexOf(e), 1);
                         }
                     };
                 },
                 8437: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.BufferLine = i.DEFAULT_ATTR_DATA = void 0;
                     const o = n(3734),
                         c = n(511),
                         a = n(643),
                         d = n(482);
                     i.DEFAULT_ATTR_DATA = Object.freeze(new o.AttributeData());
-                    let f = 0;
-                    class g {
-                        constructor(s, r, t = !1) {
-                            this.isWrapped = t, this._combined = {}, this._extendedAttrs = {}, this._data = new Uint32Array(3 * s);
-                            const e = r || c.CellData.fromCharData([0, a.NULL_CELL_CHAR, a.NULL_CELL_WIDTH, a.NULL_CELL_CODE]);
+                    let v = 0;
+                    class m {
+                        constructor(s, r, e = !1) {
+                            this.isWrapped = e, this._combined = {}, this._extendedAttrs = {}, this._data = new Uint32Array(3 * s);
+                            const t = r || c.CellData.fromCharData([0, a.NULL_CELL_CHAR, a.NULL_CELL_WIDTH, a.NULL_CELL_CODE]);
                             for (let h = 0; h < s; ++h)
-                                this.setCell(h, e);
+                                this.setCell(h, t);
                             this.length = s;
                         }
                         get(s) {
                             const r = this._data[3 * s + 0],
-                                t = 2097151 & r;
-                            return [this._data[3 * s + 1], 2097152 & r ? this._combined[s] : t ? (0, d.stringFromCodePoint)(t) : "", r >> 22, 2097152 & r ? this._combined[s].charCodeAt(this._combined[s].length - 1) : t];
+                                e = 2097151 & r;
+                            return [this._data[3 * s + 1], 2097152 & r ? this._combined[s] : e ? (0, d.stringFromCodePoint)(e) : "", r >> 22, 2097152 & r ? this._combined[s].charCodeAt(this._combined[s].length - 1) : e];
                         }
                         set(s, r) {
                             this._data[3 * s + 1] = r[a.CHAR_DATA_ATTR_INDEX], r[a.CHAR_DATA_CHAR_INDEX].length > 1 ? (this._combined[s] = r[1], this._data[3 * s + 0] = 2097152 | s | r[a.CHAR_DATA_WIDTH_INDEX] << 22) : this._data[3 * s + 0] = r[a.CHAR_DATA_CHAR_INDEX].charCodeAt(0) | r[a.CHAR_DATA_WIDTH_INDEX] << 22;
                         }
                         getWidth(s) {
                             return this._data[3 * s + 0] >> 22;
                         }
@@ -7774,114 +7774,114 @@
                             const r = this._data[3 * s + 0];
                             return 2097152 & r ? this._combined[s] : 2097151 & r ? (0, d.stringFromCodePoint)(2097151 & r) : "";
                         }
                         isProtected(s) {
                             return 536870912 & this._data[3 * s + 2];
                         }
                         loadCell(s, r) {
-                            return f = 3 * s, r.content = this._data[f + 0], r.fg = this._data[f + 1], r.bg = this._data[f + 2], 2097152 & r.content && (r.combinedData = this._combined[s]), 268435456 & r.bg && (r.extended = this._extendedAttrs[s]), r;
+                            return v = 3 * s, r.content = this._data[v + 0], r.fg = this._data[v + 1], r.bg = this._data[v + 2], 2097152 & r.content && (r.combinedData = this._combined[s]), 268435456 & r.bg && (r.extended = this._extendedAttrs[s]), r;
                         }
                         setCell(s, r) {
                             2097152 & r.content && (this._combined[s] = r.combinedData), 268435456 & r.bg && (this._extendedAttrs[s] = r.extended), this._data[3 * s + 0] = r.content, this._data[3 * s + 1] = r.fg, this._data[3 * s + 2] = r.bg;
                         }
-                        setCellFromCodepoint(s, r, t, e) {
-                            268435456 & e.bg && (this._extendedAttrs[s] = e.extended), this._data[3 * s + 0] = r | t << 22, this._data[3 * s + 1] = e.fg, this._data[3 * s + 2] = e.bg;
+                        setCellFromCodepoint(s, r, e, t) {
+                            268435456 & t.bg && (this._extendedAttrs[s] = t.extended), this._data[3 * s + 0] = r | e << 22, this._data[3 * s + 1] = t.fg, this._data[3 * s + 2] = t.bg;
                         }
-                        addCodepointToCell(s, r, t) {
-                            let e = this._data[3 * s + 0];
-                            2097152 & e ? this._combined[s] += (0, d.stringFromCodePoint)(r) : 2097151 & e ? (this._combined[s] = (0, d.stringFromCodePoint)(2097151 & e) + (0, d.stringFromCodePoint)(r), e &= -2097152, e |= 2097152) : e = r | 4194304, t && (e &= -12582913, e |= t << 22), this._data[3 * s + 0] = e;
-                        }
-                        insertCells(s, r, t) {
-                            if ((s %= this.length) && this.getWidth(s - 1) === 2 && this.setCellFromCodepoint(s - 1, 0, 1, t), r < this.length - s) {
-                                const e = new c.CellData();
+                        addCodepointToCell(s, r, e) {
+                            let t = this._data[3 * s + 0];
+                            2097152 & t ? this._combined[s] += (0, d.stringFromCodePoint)(r) : 2097151 & t ? (this._combined[s] = (0, d.stringFromCodePoint)(2097151 & t) + (0, d.stringFromCodePoint)(r), t &= -2097152, t |= 2097152) : t = r | 4194304, e && (t &= -12582913, t |= e << 22), this._data[3 * s + 0] = t;
+                        }
+                        insertCells(s, r, e) {
+                            if ((s %= this.length) && this.getWidth(s - 1) === 2 && this.setCellFromCodepoint(s - 1, 0, 1, e), r < this.length - s) {
+                                const t = new c.CellData();
                                 for (let h = this.length - s - r - 1; h >= 0; --h)
-                                    this.setCell(s + r + h, this.loadCell(s + h, e));
+                                    this.setCell(s + r + h, this.loadCell(s + h, t));
                                 for (let h = 0; h < r; ++h)
-                                    this.setCell(s + h, t);
+                                    this.setCell(s + h, e);
                             } else
-                                for (let e = s; e < this.length; ++e)
-                                    this.setCell(e, t);
-                            this.getWidth(this.length - 1) === 2 && this.setCellFromCodepoint(this.length - 1, 0, 1, t);
+                                for (let t = s; t < this.length; ++t)
+                                    this.setCell(t, e);
+                            this.getWidth(this.length - 1) === 2 && this.setCellFromCodepoint(this.length - 1, 0, 1, e);
                         }
-                        deleteCells(s, r, t) {
+                        deleteCells(s, r, e) {
                             if (s %= this.length, r < this.length - s) {
-                                const e = new c.CellData();
+                                const t = new c.CellData();
                                 for (let h = 0; h < this.length - s - r; ++h)
-                                    this.setCell(s + h, this.loadCell(s + r + h, e));
+                                    this.setCell(s + h, this.loadCell(s + r + h, t));
                                 for (let h = this.length - r; h < this.length; ++h)
-                                    this.setCell(h, t);
+                                    this.setCell(h, e);
                             } else
-                                for (let e = s; e < this.length; ++e)
-                                    this.setCell(e, t);
-                            s && this.getWidth(s - 1) === 2 && this.setCellFromCodepoint(s - 1, 0, 1, t), this.getWidth(s) !== 0 || this.hasContent(s) || this.setCellFromCodepoint(s, 0, 1, t);
-                        }
-                        replaceCells(s, r, t, e = !1) {
-                            if (e)
-                                for (s && this.getWidth(s - 1) === 2 && !this.isProtected(s - 1) && this.setCellFromCodepoint(s - 1, 0, 1, t), r < this.length && this.getWidth(r - 1) === 2 && !this.isProtected(r) && this.setCellFromCodepoint(r, 0, 1, t); s < r && s < this.length;)
-                                    this.isProtected(s) || this.setCell(s, t), s++;
+                                for (let t = s; t < this.length; ++t)
+                                    this.setCell(t, e);
+                            s && this.getWidth(s - 1) === 2 && this.setCellFromCodepoint(s - 1, 0, 1, e), this.getWidth(s) !== 0 || this.hasContent(s) || this.setCellFromCodepoint(s, 0, 1, e);
+                        }
+                        replaceCells(s, r, e, t = !1) {
+                            if (t)
+                                for (s && this.getWidth(s - 1) === 2 && !this.isProtected(s - 1) && this.setCellFromCodepoint(s - 1, 0, 1, e), r < this.length && this.getWidth(r - 1) === 2 && !this.isProtected(r) && this.setCellFromCodepoint(r, 0, 1, e); s < r && s < this.length;)
+                                    this.isProtected(s) || this.setCell(s, e), s++;
                             else
-                                for (s && this.getWidth(s - 1) === 2 && this.setCellFromCodepoint(s - 1, 0, 1, t), r < this.length && this.getWidth(r - 1) === 2 && this.setCellFromCodepoint(r, 0, 1, t); s < r && s < this.length;)
-                                    this.setCell(s++, t);
+                                for (s && this.getWidth(s - 1) === 2 && this.setCellFromCodepoint(s - 1, 0, 1, e), r < this.length && this.getWidth(r - 1) === 2 && this.setCellFromCodepoint(r, 0, 1, e); s < r && s < this.length;)
+                                    this.setCell(s++, e);
                         }
                         resize(s, r) {
                             if (s === this.length)
                                 return 4 * this._data.length * 2 < this._data.buffer.byteLength;
-                            const t = 3 * s;
+                            const e = 3 * s;
                             if (s > this.length) {
-                                if (this._data.buffer.byteLength >= 4 * t)
-                                    this._data = new Uint32Array(this._data.buffer, 0, t);
+                                if (this._data.buffer.byteLength >= 4 * e)
+                                    this._data = new Uint32Array(this._data.buffer, 0, e);
                                 else {
-                                    const e = new Uint32Array(t);
-                                    e.set(this._data), this._data = e;
+                                    const t = new Uint32Array(e);
+                                    t.set(this._data), this._data = t;
                                 }
-                                for (let e = this.length; e < s; ++e)
-                                    this.setCell(e, r);
+                                for (let t = this.length; t < s; ++t)
+                                    this.setCell(t, r);
                             } else {
-                                this._data = this._data.subarray(0, t);
-                                const e = Object.keys(this._combined);
-                                for (let v = 0; v < e.length; v++) {
-                                    const u = parseInt(e[v], 10);
+                                this._data = this._data.subarray(0, e);
+                                const t = Object.keys(this._combined);
+                                for (let g = 0; g < t.length; g++) {
+                                    const u = parseInt(t[g], 10);
                                     u >= s && delete this._combined[u];
                                 }
                                 const h = Object.keys(this._extendedAttrs);
-                                for (let v = 0; v < h.length; v++) {
-                                    const u = parseInt(h[v], 10);
+                                for (let g = 0; g < h.length; g++) {
+                                    const u = parseInt(h[g], 10);
                                     u >= s && delete this._extendedAttrs[u];
                                 }
                             }
-                            return this.length = s, 4 * t * 2 < this._data.buffer.byteLength;
+                            return this.length = s, 4 * e * 2 < this._data.buffer.byteLength;
                         }
                         cleanupMemory() {
                             if (4 * this._data.length * 2 < this._data.buffer.byteLength) {
                                 const s = new Uint32Array(this._data.length);
                                 return s.set(this._data), this._data = s, 1;
                             }
                             return 0;
                         }
                         fill(s, r = !1) {
                             if (r)
-                                for (let t = 0; t < this.length; ++t)
-                                    this.isProtected(t) || this.setCell(t, s);
+                                for (let e = 0; e < this.length; ++e)
+                                    this.isProtected(e) || this.setCell(e, s);
                             else {
                                 this._combined = {}, this._extendedAttrs = {};
-                                for (let t = 0; t < this.length; ++t)
-                                    this.setCell(t, s);
+                                for (let e = 0; e < this.length; ++e)
+                                    this.setCell(e, s);
                             }
                         }
                         copyFrom(s) {
                             this.length !== s.length ? this._data = new Uint32Array(s._data) : this._data.set(s._data), this.length = s.length, this._combined = {};
                             for (const r in s._combined)
                                 this._combined[r] = s._combined[r];
                             this._extendedAttrs = {};
                             for (const r in s._extendedAttrs)
                                 this._extendedAttrs[r] = s._extendedAttrs[r];
                             this.isWrapped = s.isWrapped;
                         }
                         clone() {
-                            const s = new g(0);
+                            const s = new m(0);
                             s._data = new Uint32Array(this._data), s.length = this.length;
                             for (const r in this._combined)
                                 s._combined[r] = this._combined[r];
                             for (const r in this._extendedAttrs)
                                 s._extendedAttrs[r] = this._extendedAttrs[r];
                             return s.isWrapped = this.isWrapped, s;
                         }
@@ -7893,50 +7893,50 @@
                         }
                         getNoBgTrimmedLength() {
                             for (let s = this.length - 1; s >= 0; --s)
                                 if (4194303 & this._data[3 * s + 0] || 50331648 & this._data[3 * s + 2])
                                     return s + (this._data[3 * s + 0] >> 22);
                             return 0;
                         }
-                        copyCellsFrom(s, r, t, e, h) {
-                            const v = s._data;
+                        copyCellsFrom(s, r, e, t, h) {
+                            const g = s._data;
                             if (h)
-                                for (let p = e - 1; p >= 0; p--) {
+                                for (let S = t - 1; S >= 0; S--) {
                                     for (let _ = 0; _ < 3; _++)
-                                        this._data[3 * (t + p) + _] = v[3 * (r + p) + _];
-                                    268435456 & v[3 * (r + p) + 2] && (this._extendedAttrs[t + p] = s._extendedAttrs[r + p]);
+                                        this._data[3 * (e + S) + _] = g[3 * (r + S) + _];
+                                    268435456 & g[3 * (r + S) + 2] && (this._extendedAttrs[e + S] = s._extendedAttrs[r + S]);
                                 }
                             else
-                                for (let p = 0; p < e; p++) {
+                                for (let S = 0; S < t; S++) {
                                     for (let _ = 0; _ < 3; _++)
-                                        this._data[3 * (t + p) + _] = v[3 * (r + p) + _];
-                                    268435456 & v[3 * (r + p) + 2] && (this._extendedAttrs[t + p] = s._extendedAttrs[r + p]);
+                                        this._data[3 * (e + S) + _] = g[3 * (r + S) + _];
+                                    268435456 & g[3 * (r + S) + 2] && (this._extendedAttrs[e + S] = s._extendedAttrs[r + S]);
                                 }
                             const u = Object.keys(s._combined);
-                            for (let p = 0; p < u.length; p++) {
-                                const _ = parseInt(u[p], 10);
-                                _ >= r && (this._combined[_ - r + t] = s._combined[_]);
+                            for (let S = 0; S < u.length; S++) {
+                                const _ = parseInt(u[S], 10);
+                                _ >= r && (this._combined[_ - r + e] = s._combined[_]);
                             }
                         }
-                        translateToString(s, r, t, e) {
-                            r = r ?? 0, t = t ?? this.length, s && (t = Math.min(t, this.getTrimmedLength())), e && (e.length = 0);
+                        translateToString(s, r, e, t) {
+                            r = r ?? 0, e = e ?? this.length, s && (e = Math.min(e, this.getTrimmedLength())), t && (t.length = 0);
                             let h = "";
-                            for (; r < t;) {
-                                const v = this._data[3 * r + 0],
-                                    u = 2097151 & v,
-                                    p = 2097152 & v ? this._combined[r] : u ? (0, d.stringFromCodePoint)(u) : a.WHITESPACE_CELL_CHAR;
-                                if (h += p, e)
-                                    for (let _ = 0; _ < p.length; ++_)
-                                        e.push(r);
-                                r += v >> 22 || 1;
+                            for (; r < e;) {
+                                const g = this._data[3 * r + 0],
+                                    u = 2097151 & g,
+                                    S = 2097152 & g ? this._combined[r] : u ? (0, d.stringFromCodePoint)(u) : a.WHITESPACE_CELL_CHAR;
+                                if (h += S, t)
+                                    for (let _ = 0; _ < S.length; ++_)
+                                        t.push(r);
+                                r += g >> 22 || 1;
                             }
-                            return e && e.push(r), h;
+                            return t && t.push(r), h;
                         }
                     }
-                    i.BufferLine = g;
+                    i.BufferLine = m;
                 },
                 4841: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.getRangeLength = void 0, i.getRangeLength = function(n, o) {
                         if (n.start.y > n.end.y)
                             throw new Error(`Buffer range end (${n.end.x}, ${n.end.y}) cannot be before start (${n.start.x}, ${n.start.y})`);
@@ -7944,108 +7944,108 @@
                     };
                 },
                 4634: (k, i) => {
                     function n(o, c, a) {
                         if (c === o.length - 1)
                             return o[c].getTrimmedLength();
                         const d = !o[c].hasContent(a - 1) && o[c].getWidth(a - 1) === 1,
-                            f = o[c + 1].getWidth(0) === 2;
-                        return d && f ? a - 1 : a;
+                            v = o[c + 1].getWidth(0) === 2;
+                        return d && v ? a - 1 : a;
                     }
                     Object.defineProperty(i, "__esModule", {
                         value: !0
-                    }), i.getWrappedLineTrimmedLength = i.reflowSmallerGetNewLineLengths = i.reflowLargerApplyNewLayout = i.reflowLargerCreateNewLayout = i.reflowLargerGetLinesToRemove = void 0, i.reflowLargerGetLinesToRemove = function(o, c, a, d, f) {
-                        const g = [];
+                    }), i.getWrappedLineTrimmedLength = i.reflowSmallerGetNewLineLengths = i.reflowLargerApplyNewLayout = i.reflowLargerCreateNewLayout = i.reflowLargerGetLinesToRemove = void 0, i.reflowLargerGetLinesToRemove = function(o, c, a, d, v) {
+                        const m = [];
                         for (let l = 0; l < o.length - 1; l++) {
                             let s = l,
                                 r = o.get(++s);
                             if (!r.isWrapped)
                                 continue;
-                            const t = [o.get(l)];
+                            const e = [o.get(l)];
                             for (; s < o.length && r.isWrapped;)
-                                t.push(r), r = o.get(++s);
+                                e.push(r), r = o.get(++s);
                             if (d >= l && d < s) {
-                                l += t.length - 1;
+                                l += e.length - 1;
                                 continue;
                             }
-                            let e = 0,
-                                h = n(t, e, c),
-                                v = 1,
+                            let t = 0,
+                                h = n(e, t, c),
+                                g = 1,
                                 u = 0;
-                            for (; v < t.length;) {
-                                const _ = n(t, v, c),
+                            for (; g < e.length;) {
+                                const _ = n(e, g, c),
                                     b = _ - u,
-                                    A = a - h,
-                                    T = Math.min(b, A);
-                                t[e].copyCellsFrom(t[v], u, h, T, !1), h += T, h === a && (e++, h = 0), u += T, u === _ && (v++, u = 0), h === 0 && e !== 0 && t[e - 1].getWidth(a - 1) === 2 && (t[e].copyCellsFrom(t[e - 1], a - 1, h++, 1, !1), t[e - 1].setCell(a - 1, f));
-                            }
-                            t[e].replaceCells(h, a, f);
-                            let p = 0;
-                            for (let _ = t.length - 1; _ > 0 && (_ > e || t[_].getTrimmedLength() === 0); _--)
-                                p++;
-                            p > 0 && (g.push(l + t.length - p), g.push(p)), l += t.length - 1;
+                                    R = a - h,
+                                    B = Math.min(b, R);
+                                e[t].copyCellsFrom(e[g], u, h, B, !1), h += B, h === a && (t++, h = 0), u += B, u === _ && (g++, u = 0), h === 0 && t !== 0 && e[t - 1].getWidth(a - 1) === 2 && (e[t].copyCellsFrom(e[t - 1], a - 1, h++, 1, !1), e[t - 1].setCell(a - 1, v));
+                            }
+                            e[t].replaceCells(h, a, v);
+                            let S = 0;
+                            for (let _ = e.length - 1; _ > 0 && (_ > t || e[_].getTrimmedLength() === 0); _--)
+                                S++;
+                            S > 0 && (m.push(l + e.length - S), m.push(S)), l += e.length - 1;
                         }
-                        return g;
+                        return m;
                     }, i.reflowLargerCreateNewLayout = function(o, c) {
                         const a = [];
                         let d = 0,
-                            f = c[d],
-                            g = 0;
+                            v = c[d],
+                            m = 0;
                         for (let l = 0; l < o.length; l++)
-                            if (f === l) {
+                            if (v === l) {
                                 const s = c[++d];
                                 o.onDeleteEmitter.fire({
-                                    index: l - g,
+                                    index: l - m,
                                     amount: s
-                                }), l += s - 1, g += s, f = c[++d];
+                                }), l += s - 1, m += s, v = c[++d];
                             } else
                                 a.push(l);
                         return {
                             layout: a,
-                            countRemoved: g
+                            countRemoved: m
                         };
                     }, i.reflowLargerApplyNewLayout = function(o, c) {
                         const a = [];
                         for (let d = 0; d < c.length; d++)
                             a.push(o.get(c[d]));
                         for (let d = 0; d < a.length; d++)
                             o.set(d, a[d]);
                         o.length = c.length;
                     }, i.reflowSmallerGetNewLineLengths = function(o, c, a) {
                         const d = [],
-                            f = o.map((r, t) => n(o, t, c)).reduce((r, t) => r + t);
-                        let g = 0,
+                            v = o.map((r, e) => n(o, e, c)).reduce((r, e) => r + e);
+                        let m = 0,
                             l = 0,
                             s = 0;
-                        for (; s < f;) {
-                            if (f - s < a) {
-                                d.push(f - s);
+                        for (; s < v;) {
+                            if (v - s < a) {
+                                d.push(v - s);
                                 break;
                             }
-                            g += a;
+                            m += a;
                             const r = n(o, l, c);
-                            g > r && (g -= r, l++);
-                            const t = o[l].getWidth(g - 1) === 2;
-                            t && g--;
-                            const e = t ? a - 1 : a;
-                            d.push(e), s += e;
+                            m > r && (m -= r, l++);
+                            const e = o[l].getWidth(m - 1) === 2;
+                            e && m--;
+                            const t = e ? a - 1 : a;
+                            d.push(t), s += t;
                         }
                         return d;
                     }, i.getWrappedLineTrimmedLength = n;
                 },
                 5295: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.BufferSet = void 0;
                     const o = n(8460),
                         c = n(844),
                         a = n(9092);
                     class d extends c.Disposable {
-                        constructor(g, l) {
-                            super(), this._optionsService = g, this._bufferService = l, this._onBufferActivate = this.register(new o.EventEmitter()), this.onBufferActivate = this._onBufferActivate.event, this.reset(), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.resize(this._bufferService.cols, this._bufferService.rows))), this.register(this._optionsService.onSpecificOptionChange("tabStopWidth", () => this.setupTabStops()));
+                        constructor(m, l) {
+                            super(), this._optionsService = m, this._bufferService = l, this._onBufferActivate = this.register(new o.EventEmitter()), this.onBufferActivate = this._onBufferActivate.event, this.reset(), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.resize(this._bufferService.cols, this._bufferService.rows))), this.register(this._optionsService.onSpecificOptionChange("tabStopWidth", () => this.setupTabStops()));
                         }
                         reset() {
                             this._normal = new a.Buffer(!0, this._optionsService, this._bufferService), this._normal.fillViewportRows(), this._alt = new a.Buffer(!1, this._optionsService, this._bufferService), this._activeBuffer = this._normal, this._onBufferActivate.fire({
                                 activeBuffer: this._normal,
                                 inactiveBuffer: this._alt
                             }), this.setupTabStops();
                         }
@@ -8060,25 +8060,25 @@
                         }
                         activateNormalBuffer() {
                             this._activeBuffer !== this._normal && (this._normal.x = this._alt.x, this._normal.y = this._alt.y, this._alt.clearAllMarkers(), this._alt.clear(), this._activeBuffer = this._normal, this._onBufferActivate.fire({
                                 activeBuffer: this._normal,
                                 inactiveBuffer: this._alt
                             }));
                         }
-                        activateAltBuffer(g) {
-                            this._activeBuffer !== this._alt && (this._alt.fillViewportRows(g), this._alt.x = this._normal.x, this._alt.y = this._normal.y, this._activeBuffer = this._alt, this._onBufferActivate.fire({
+                        activateAltBuffer(m) {
+                            this._activeBuffer !== this._alt && (this._alt.fillViewportRows(m), this._alt.x = this._normal.x, this._alt.y = this._normal.y, this._activeBuffer = this._alt, this._onBufferActivate.fire({
                                 activeBuffer: this._alt,
                                 inactiveBuffer: this._normal
                             }));
                         }
-                        resize(g, l) {
-                            this._normal.resize(g, l), this._alt.resize(g, l), this.setupTabStops(g);
+                        resize(m, l) {
+                            this._normal.resize(m, l), this._alt.resize(m, l), this.setupTabStops(m);
                         }
-                        setupTabStops(g) {
-                            this._normal.setupTabStops(g), this._alt.setupTabStops(g);
+                        setupTabStops(m) {
+                            this._normal.setupTabStops(m), this._alt.setupTabStops(m);
                         }
                     }
                     i.BufferSet = d;
                 },
                 511: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
@@ -8086,45 +8086,45 @@
                     const o = n(482),
                         c = n(643),
                         a = n(3734);
                     class d extends a.AttributeData {
                         constructor() {
                             super(...arguments), this.content = 0, this.fg = 0, this.bg = 0, this.extended = new a.ExtendedAttrs(), this.combinedData = "";
                         }
-                        static fromCharData(g) {
+                        static fromCharData(m) {
                             const l = new d();
-                            return l.setFromCharData(g), l;
+                            return l.setFromCharData(m), l;
                         }
                         isCombined() {
                             return 2097152 & this.content;
                         }
                         getWidth() {
                             return this.content >> 22;
                         }
                         getChars() {
                             return 2097152 & this.content ? this.combinedData : 2097151 & this.content ? (0, o.stringFromCodePoint)(2097151 & this.content) : "";
                         }
                         getCode() {
                             return this.isCombined() ? this.combinedData.charCodeAt(this.combinedData.length - 1) : 2097151 & this.content;
                         }
-                        setFromCharData(g) {
-                            this.fg = g[c.CHAR_DATA_ATTR_INDEX], this.bg = 0;
+                        setFromCharData(m) {
+                            this.fg = m[c.CHAR_DATA_ATTR_INDEX], this.bg = 0;
                             let l = !1;
-                            if (g[c.CHAR_DATA_CHAR_INDEX].length > 2)
+                            if (m[c.CHAR_DATA_CHAR_INDEX].length > 2)
                                 l = !0;
-                            else if (g[c.CHAR_DATA_CHAR_INDEX].length === 2) {
-                                const s = g[c.CHAR_DATA_CHAR_INDEX].charCodeAt(0);
+                            else if (m[c.CHAR_DATA_CHAR_INDEX].length === 2) {
+                                const s = m[c.CHAR_DATA_CHAR_INDEX].charCodeAt(0);
                                 if (55296 <= s && s <= 56319) {
-                                    const r = g[c.CHAR_DATA_CHAR_INDEX].charCodeAt(1);
-                                    56320 <= r && r <= 57343 ? this.content = 1024 * (s - 55296) + r - 56320 + 65536 | g[c.CHAR_DATA_WIDTH_INDEX] << 22 : l = !0;
+                                    const r = m[c.CHAR_DATA_CHAR_INDEX].charCodeAt(1);
+                                    56320 <= r && r <= 57343 ? this.content = 1024 * (s - 55296) + r - 56320 + 65536 | m[c.CHAR_DATA_WIDTH_INDEX] << 22 : l = !0;
                                 } else
                                     l = !0;
                             } else
-                                this.content = g[c.CHAR_DATA_CHAR_INDEX].charCodeAt(0) | g[c.CHAR_DATA_WIDTH_INDEX] << 22;
-                            l && (this.combinedData = g[c.CHAR_DATA_CHAR_INDEX], this.content = 2097152 | g[c.CHAR_DATA_WIDTH_INDEX] << 22);
+                                this.content = m[c.CHAR_DATA_CHAR_INDEX].charCodeAt(0) | m[c.CHAR_DATA_WIDTH_INDEX] << 22;
+                            l && (this.combinedData = m[c.CHAR_DATA_CHAR_INDEX], this.content = 2097152 | m[c.CHAR_DATA_WIDTH_INDEX] << 22);
                         }
                         getAsCharData() {
                             return [this.fg, this.getChars(), this.getWidth(), this.getCode()];
                         }
                     }
                     i.CellData = d;
                 },
@@ -8139,22 +8139,22 @@
                     }), i.Marker = void 0;
                     const o = n(8460),
                         c = n(844);
                     class a {
                         get id() {
                             return this._id;
                         }
-                        constructor(f) {
-                            this.line = f, this.isDisposed = !1, this._disposables = [], this._id = a._nextId++, this._onDispose = this.register(new o.EventEmitter()), this.onDispose = this._onDispose.event;
+                        constructor(v) {
+                            this.line = v, this.isDisposed = !1, this._disposables = [], this._id = a._nextId++, this._onDispose = this.register(new o.EventEmitter()), this.onDispose = this._onDispose.event;
                         }
                         dispose() {
                             this.isDisposed || (this.isDisposed = !0, this.line = -1, this._onDispose.fire(), (0, c.disposeArray)(this._disposables), this._disposables.length = 0);
                         }
-                        register(f) {
-                            return this._disposables.push(f), f;
+                        register(v) {
+                            return this._disposables.push(v), v;
                         }
                     }
                     i.Marker = a, a._nextId = 1;
                 },
                 7116: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
@@ -8339,15 +8339,15 @@
                             191: ["/", "?"],
                             192: ["`", "~"],
                             219: ["[", "{"],
                             220: ["\\", "|"],
                             221: ["]", "}"],
                             222: ["'", '"']
                         };
-                    i.evaluateKeyboardEvent = function(a, d, f, g) {
+                    i.evaluateKeyboardEvent = function(a, d, v, m) {
                         const l = {
                                 type: 0,
                                 cancel: !1,
                                 key: void 0
                             },
                             s = (a.shiftKey ? 1 : 0) | (a.altKey ? 2 : 0) | (a.ctrlKey ? 4 : 0) | (a.metaKey ? 8 : 0);
                         switch (a.keyCode) {
@@ -8369,30 +8369,30 @@
                                 break;
                             case 27:
                                 l.key = o.C0.ESC, a.altKey && (l.key = o.C0.ESC + o.C0.ESC), l.cancel = !0;
                                 break;
                             case 37:
                                 if (a.metaKey)
                                     break;
-                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "D", l.key === o.C0.ESC + "[1;3D" && (l.key = o.C0.ESC + (f ? "b" : "[1;5D"))) : l.key = d ? o.C0.ESC + "OD" : o.C0.ESC + "[D";
+                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "D", l.key === o.C0.ESC + "[1;3D" && (l.key = o.C0.ESC + (v ? "b" : "[1;5D"))) : l.key = d ? o.C0.ESC + "OD" : o.C0.ESC + "[D";
                                 break;
                             case 39:
                                 if (a.metaKey)
                                     break;
-                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "C", l.key === o.C0.ESC + "[1;3C" && (l.key = o.C0.ESC + (f ? "f" : "[1;5C"))) : l.key = d ? o.C0.ESC + "OC" : o.C0.ESC + "[C";
+                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "C", l.key === o.C0.ESC + "[1;3C" && (l.key = o.C0.ESC + (v ? "f" : "[1;5C"))) : l.key = d ? o.C0.ESC + "OC" : o.C0.ESC + "[C";
                                 break;
                             case 38:
                                 if (a.metaKey)
                                     break;
-                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "A", f || l.key !== o.C0.ESC + "[1;3A" || (l.key = o.C0.ESC + "[1;5A")) : l.key = d ? o.C0.ESC + "OA" : o.C0.ESC + "[A";
+                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "A", v || l.key !== o.C0.ESC + "[1;3A" || (l.key = o.C0.ESC + "[1;5A")) : l.key = d ? o.C0.ESC + "OA" : o.C0.ESC + "[A";
                                 break;
                             case 40:
                                 if (a.metaKey)
                                     break;
-                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "B", f || l.key !== o.C0.ESC + "[1;3B" || (l.key = o.C0.ESC + "[1;5B")) : l.key = d ? o.C0.ESC + "OB" : o.C0.ESC + "[B";
+                                s ? (l.key = o.C0.ESC + "[1;" + (s + 1) + "B", v || l.key !== o.C0.ESC + "[1;3B" || (l.key = o.C0.ESC + "[1;5B")) : l.key = d ? o.C0.ESC + "OB" : o.C0.ESC + "[B";
                                 break;
                             case 45:
                                 a.shiftKey || a.ctrlKey || (l.key = o.C0.ESC + "[2~");
                                 break;
                             case 46:
                                 l.key = s ? o.C0.ESC + "[3;" + (s + 1) + "~" : o.C0.ESC + "[3~";
                                 break;
@@ -8442,30 +8442,30 @@
                                 l.key = s ? o.C0.ESC + "[23;" + (s + 1) + "~" : o.C0.ESC + "[23~";
                                 break;
                             case 123:
                                 l.key = s ? o.C0.ESC + "[24;" + (s + 1) + "~" : o.C0.ESC + "[24~";
                                 break;
                             default:
                                 if (!a.ctrlKey || a.shiftKey || a.altKey || a.metaKey)
-                                    if (f && !g || !a.altKey || a.metaKey)
-                                        !f || a.altKey || a.ctrlKey || a.shiftKey || !a.metaKey ? a.key && !a.ctrlKey && !a.altKey && !a.metaKey && a.keyCode >= 48 && a.key.length === 1 ? l.key = a.key : a.key && a.ctrlKey && (a.key === "_" && (l.key = o.C0.US), a.key === "@" && (l.key = o.C0.NUL)) : a.keyCode === 65 && (l.type = 1);
+                                    if (v && !m || !a.altKey || a.metaKey)
+                                        !v || a.altKey || a.ctrlKey || a.shiftKey || !a.metaKey ? a.key && !a.ctrlKey && !a.altKey && !a.metaKey && a.keyCode >= 48 && a.key.length === 1 ? l.key = a.key : a.key && a.ctrlKey && (a.key === "_" && (l.key = o.C0.US), a.key === "@" && (l.key = o.C0.NUL)) : a.keyCode === 65 && (l.type = 1);
                                     else {
                                         const r = c[a.keyCode],
-                                            t = r == null ? void 0 : r[a.shiftKey ? 1 : 0];
-                                        if (t)
-                                            l.key = o.C0.ESC + t;
+                                            e = r == null ? void 0 : r[a.shiftKey ? 1 : 0];
+                                        if (e)
+                                            l.key = o.C0.ESC + e;
                                         else if (a.keyCode >= 65 && a.keyCode <= 90) {
-                                            const e = a.ctrlKey ? a.keyCode - 64 : a.keyCode + 32;
-                                            let h = String.fromCharCode(e);
+                                            const t = a.ctrlKey ? a.keyCode - 64 : a.keyCode + 32;
+                                            let h = String.fromCharCode(t);
                                             a.shiftKey && (h = h.toUpperCase()), l.key = o.C0.ESC + h;
                                         } else if (a.keyCode === 32)
                                             l.key = o.C0.ESC + (a.ctrlKey ? o.C0.NUL : " ");
                                         else if (a.key === "Dead" && a.code.startsWith("Key")) {
-                                            let e = a.code.slice(3, 4);
-                                            a.shiftKey || (e = e.toLowerCase()), l.key = o.C0.ESC + e, l.cancel = !0;
+                                            let t = a.code.slice(3, 4);
+                                            a.shiftKey || (t = t.toLowerCase()), l.key = o.C0.ESC + t, l.cancel = !0;
                                         }
                                     }
                                 else
                                     a.keyCode >= 65 && a.keyCode <= 90 ? l.key = String.fromCharCode(a.keyCode - 64) : a.keyCode === 32 ? l.key = o.C0.NUL : a.keyCode >= 51 && a.keyCode <= 55 ? l.key = String.fromCharCode(a.keyCode - 51 + 27) : a.keyCode === 56 ? l.key = o.C0.DEL : a.keyCode === 219 ? l.key = o.C0.ESC : a.keyCode === 220 ? l.key = o.C0.FS : a.keyCode === 221 && (l.key = o.C0.GS);
                         }
                         return l;
                     };
@@ -8474,16 +8474,16 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.Utf8ToUtf32 = i.StringToUtf32 = i.utf32ToString = i.stringFromCodePoint = void 0, i.stringFromCodePoint = function(n) {
                         return n > 65535 ? (n -= 65536, String.fromCharCode(55296 + (n >> 10)) + String.fromCharCode(n % 1024 + 56320)) : String.fromCharCode(n);
                     }, i.utf32ToString = function(n, o = 0, c = n.length) {
                         let a = "";
                         for (let d = o; d < c; ++d) {
-                            let f = n[d];
-                            f > 65535 ? (f -= 65536, a += String.fromCharCode(55296 + (f >> 10)) + String.fromCharCode(f % 1024 + 56320)) : a += String.fromCharCode(f);
+                            let v = n[d];
+                            v > 65535 ? (v -= 65536, a += String.fromCharCode(55296 + (v >> 10)) + String.fromCharCode(v % 1024 + 56320)) : a += String.fromCharCode(v);
                         }
                         return a;
                     }, i.StringToUtf32 = class {
                         constructor() {
                             this._interim = 0;
                         }
                         clear() {
@@ -8492,119 +8492,119 @@
                         decode(n, o) {
                             const c = n.length;
                             if (!c)
                                 return 0;
                             let a = 0,
                                 d = 0;
                             if (this._interim) {
-                                const f = n.charCodeAt(d++);
-                                56320 <= f && f <= 57343 ? o[a++] = 1024 * (this._interim - 55296) + f - 56320 + 65536 : (o[a++] = this._interim, o[a++] = f), this._interim = 0;
+                                const v = n.charCodeAt(d++);
+                                56320 <= v && v <= 57343 ? o[a++] = 1024 * (this._interim - 55296) + v - 56320 + 65536 : (o[a++] = this._interim, o[a++] = v), this._interim = 0;
                             }
-                            for (let f = d; f < c; ++f) {
-                                const g = n.charCodeAt(f);
-                                if (55296 <= g && g <= 56319) {
-                                    if (++f >= c)
-                                        return this._interim = g, a;
-                                    const l = n.charCodeAt(f);
-                                    56320 <= l && l <= 57343 ? o[a++] = 1024 * (g - 55296) + l - 56320 + 65536 : (o[a++] = g, o[a++] = l);
+                            for (let v = d; v < c; ++v) {
+                                const m = n.charCodeAt(v);
+                                if (55296 <= m && m <= 56319) {
+                                    if (++v >= c)
+                                        return this._interim = m, a;
+                                    const l = n.charCodeAt(v);
+                                    56320 <= l && l <= 57343 ? o[a++] = 1024 * (m - 55296) + l - 56320 + 65536 : (o[a++] = m, o[a++] = l);
                                 } else
-                                    g !== 65279 && (o[a++] = g);
+                                    m !== 65279 && (o[a++] = m);
                             }
                             return a;
                         }
                     }, i.Utf8ToUtf32 = class {
                         constructor() {
                             this.interim = new Uint8Array(3);
                         }
                         clear() {
                             this.interim.fill(0);
                         }
                         decode(n, o) {
                             const c = n.length;
                             if (!c)
                                 return 0;
-                            let a, d, f, g, l = 0,
+                            let a, d, v, m, l = 0,
                                 s = 0,
                                 r = 0;
                             if (this.interim[0]) {
                                 let h = !1,
-                                    v = this.interim[0];
-                                v &= (224 & v) == 192 ? 31 : (240 & v) == 224 ? 15 : 7;
-                                let u, p = 0;
+                                    g = this.interim[0];
+                                g &= (224 & g) == 192 ? 31 : (240 & g) == 224 ? 15 : 7;
+                                let u, S = 0;
                                 for (;
-                                    (u = 63 & this.interim[++p]) && p < 4;)
-                                    v <<= 6, v |= u;
+                                    (u = 63 & this.interim[++S]) && S < 4;)
+                                    g <<= 6, g |= u;
                                 const _ = (224 & this.interim[0]) == 192 ? 2 : (240 & this.interim[0]) == 224 ? 3 : 4,
-                                    b = _ - p;
+                                    b = _ - S;
                                 for (; r < b;) {
                                     if (r >= c)
                                         return 0;
                                     if (u = n[r++], (192 & u) != 128) {
                                         r--, h = !0;
                                         break;
                                     }
-                                    this.interim[p++] = u, v <<= 6, v |= 63 & u;
+                                    this.interim[S++] = u, g <<= 6, g |= 63 & u;
                                 }
-                                h || (_ === 2 ? v < 128 ? r-- : o[l++] = v : _ === 3 ? v < 2048 || v >= 55296 && v <= 57343 || v === 65279 || (o[l++] = v) : v < 65536 || v > 1114111 || (o[l++] = v)), this.interim.fill(0);
+                                h || (_ === 2 ? g < 128 ? r-- : o[l++] = g : _ === 3 ? g < 2048 || g >= 55296 && g <= 57343 || g === 65279 || (o[l++] = g) : g < 65536 || g > 1114111 || (o[l++] = g)), this.interim.fill(0);
                             }
-                            const t = c - 4;
-                            let e = r;
-                            for (; e < c;) {
-                                for (; !(!(e < t) || 128 & (a = n[e]) || 128 & (d = n[e + 1]) || 128 & (f = n[e + 2]) || 128 & (g = n[e + 3]));)
-                                    o[l++] = a, o[l++] = d, o[l++] = f, o[l++] = g, e += 4;
-                                if (a = n[e++], a < 128)
+                            const e = c - 4;
+                            let t = r;
+                            for (; t < c;) {
+                                for (; !(!(t < e) || 128 & (a = n[t]) || 128 & (d = n[t + 1]) || 128 & (v = n[t + 2]) || 128 & (m = n[t + 3]));)
+                                    o[l++] = a, o[l++] = d, o[l++] = v, o[l++] = m, t += 4;
+                                if (a = n[t++], a < 128)
                                     o[l++] = a;
                                 else if ((224 & a) == 192) {
-                                    if (e >= c)
+                                    if (t >= c)
                                         return this.interim[0] = a, l;
-                                    if (d = n[e++], (192 & d) != 128) {
-                                        e--;
+                                    if (d = n[t++], (192 & d) != 128) {
+                                        t--;
                                         continue;
                                     }
                                     if (s = (31 & a) << 6 | 63 & d, s < 128) {
-                                        e--;
+                                        t--;
                                         continue;
                                     }
                                     o[l++] = s;
                                 } else if ((240 & a) == 224) {
-                                    if (e >= c)
+                                    if (t >= c)
                                         return this.interim[0] = a, l;
-                                    if (d = n[e++], (192 & d) != 128) {
-                                        e--;
+                                    if (d = n[t++], (192 & d) != 128) {
+                                        t--;
                                         continue;
                                     }
-                                    if (e >= c)
+                                    if (t >= c)
                                         return this.interim[0] = a, this.interim[1] = d, l;
-                                    if (f = n[e++], (192 & f) != 128) {
-                                        e--;
+                                    if (v = n[t++], (192 & v) != 128) {
+                                        t--;
                                         continue;
                                     }
-                                    if (s = (15 & a) << 12 | (63 & d) << 6 | 63 & f, s < 2048 || s >= 55296 && s <= 57343 || s === 65279)
+                                    if (s = (15 & a) << 12 | (63 & d) << 6 | 63 & v, s < 2048 || s >= 55296 && s <= 57343 || s === 65279)
                                         continue;
                                     o[l++] = s;
                                 } else if ((248 & a) == 240) {
-                                    if (e >= c)
+                                    if (t >= c)
                                         return this.interim[0] = a, l;
-                                    if (d = n[e++], (192 & d) != 128) {
-                                        e--;
+                                    if (d = n[t++], (192 & d) != 128) {
+                                        t--;
                                         continue;
                                     }
-                                    if (e >= c)
+                                    if (t >= c)
                                         return this.interim[0] = a, this.interim[1] = d, l;
-                                    if (f = n[e++], (192 & f) != 128) {
-                                        e--;
+                                    if (v = n[t++], (192 & v) != 128) {
+                                        t--;
                                         continue;
                                     }
-                                    if (e >= c)
-                                        return this.interim[0] = a, this.interim[1] = d, this.interim[2] = f, l;
-                                    if (g = n[e++], (192 & g) != 128) {
-                                        e--;
+                                    if (t >= c)
+                                        return this.interim[0] = a, this.interim[1] = d, this.interim[2] = v, l;
+                                    if (m = n[t++], (192 & m) != 128) {
+                                        t--;
                                         continue;
                                     }
-                                    if (s = (7 & a) << 18 | (63 & d) << 12 | (63 & f) << 6 | 63 & g, s < 65536 || s > 1114111)
+                                    if (s = (7 & a) << 18 | (63 & d) << 12 | (63 & v) << 6 | 63 & m, s < 65536 || s > 1114111)
                                         continue;
                                     o[l++] = s;
                                 }
                             }
                             return l;
                         }
                     };
@@ -8761,95 +8761,95 @@
                             [917760, 917999]
                         ];
                     let d;
                     i.UnicodeV6 = class {
                         constructor() {
                             if (this.version = "6", !d) {
                                 d = new Uint8Array(65536), d.fill(1), d[0] = 0, d.fill(0, 1, 32), d.fill(0, 127, 160), d.fill(2, 4352, 4448), d[9001] = 2, d[9002] = 2, d.fill(2, 11904, 42192), d[12351] = 1, d.fill(2, 44032, 55204), d.fill(2, 63744, 64256), d.fill(2, 65040, 65050), d.fill(2, 65072, 65136), d.fill(2, 65280, 65377), d.fill(2, 65504, 65511);
-                                for (let f = 0; f < c.length; ++f)
-                                    d.fill(0, c[f][0], c[f][1] + 1);
+                                for (let v = 0; v < c.length; ++v)
+                                    d.fill(0, c[v][0], c[v][1] + 1);
                             }
                         }
-                        wcwidth(f) {
-                            return f < 32 ? 0 : f < 127 ? 1 : f < 65536 ? d[f] : function(g, l) {
+                        wcwidth(v) {
+                            return v < 32 ? 0 : v < 127 ? 1 : v < 65536 ? d[v] : function(m, l) {
                                 let s, r = 0,
-                                    t = l.length - 1;
-                                if (g < l[0][0] || g > l[t][1])
+                                    e = l.length - 1;
+                                if (m < l[0][0] || m > l[e][1])
                                     return !1;
-                                for (; t >= r;)
-                                    if (s = r + t >> 1, g > l[s][1])
+                                for (; e >= r;)
+                                    if (s = r + e >> 1, m > l[s][1])
                                         r = s + 1;
                                     else {
-                                        if (!(g < l[s][0]))
+                                        if (!(m < l[s][0]))
                                             return !0;
-                                        t = s - 1;
+                                        e = s - 1;
                                     }
                                 return !1;
-                            }(f, a) ? 0 : f >= 131072 && f <= 196605 || f >= 196608 && f <= 262141 ? 2 : 1;
+                            }(v, a) ? 0 : v >= 131072 && v <= 196605 || v >= 196608 && v <= 262141 ? 2 : 1;
                         }
-                        charProperties(f, g) {
-                            let l = this.wcwidth(f),
-                                s = l === 0 && g !== 0;
+                        charProperties(v, m) {
+                            let l = this.wcwidth(v),
+                                s = l === 0 && m !== 0;
                             if (s) {
-                                const r = o.UnicodeService.extractWidth(g);
+                                const r = o.UnicodeService.extractWidth(m);
                                 r === 0 ? s = !1 : r > l && (l = r);
                             }
                             return o.UnicodeService.createPropertyValue(0, l, s);
                         }
                     };
                 },
                 5981: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.WriteBuffer = void 0;
                     const o = n(8460),
                         c = n(844);
                     class a extends c.Disposable {
-                        constructor(f) {
-                            super(), this._action = f, this._writeBuffer = [], this._callbacks = [], this._pendingData = 0, this._bufferOffset = 0, this._isSyncWriting = !1, this._syncCalls = 0, this._didUserInput = !1, this._onWriteParsed = this.register(new o.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event;
+                        constructor(v) {
+                            super(), this._action = v, this._writeBuffer = [], this._callbacks = [], this._pendingData = 0, this._bufferOffset = 0, this._isSyncWriting = !1, this._syncCalls = 0, this._didUserInput = !1, this._onWriteParsed = this.register(new o.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event;
                         }
                         handleUserInput() {
                             this._didUserInput = !0;
                         }
-                        writeSync(f, g) {
-                            if (g !== void 0 && this._syncCalls > g)
+                        writeSync(v, m) {
+                            if (m !== void 0 && this._syncCalls > m)
                                 return void(this._syncCalls = 0);
-                            if (this._pendingData += f.length, this._writeBuffer.push(f), this._callbacks.push(void 0), this._syncCalls++, this._isSyncWriting)
+                            if (this._pendingData += v.length, this._writeBuffer.push(v), this._callbacks.push(void 0), this._syncCalls++, this._isSyncWriting)
                                 return;
                             let l;
                             for (this._isSyncWriting = !0; l = this._writeBuffer.shift();) {
                                 this._action(l);
                                 const s = this._callbacks.shift();
                                 s && s();
                             }
                             this._pendingData = 0, this._bufferOffset = 2147483647, this._isSyncWriting = !1, this._syncCalls = 0;
                         }
-                        write(f, g) {
+                        write(v, m) {
                             if (this._pendingData > 5e7)
                                 throw new Error("write data discarded, use flow control to avoid losing data");
                             if (!this._writeBuffer.length) {
                                 if (this._bufferOffset = 0, this._didUserInput)
-                                    return this._didUserInput = !1, this._pendingData += f.length, this._writeBuffer.push(f), this._callbacks.push(g), void this._innerWrite();
+                                    return this._didUserInput = !1, this._pendingData += v.length, this._writeBuffer.push(v), this._callbacks.push(m), void this._innerWrite();
                                 setTimeout(() => this._innerWrite());
                             }
-                            this._pendingData += f.length, this._writeBuffer.push(f), this._callbacks.push(g);
+                            this._pendingData += v.length, this._writeBuffer.push(v), this._callbacks.push(m);
                         }
-                        _innerWrite(f = 0, g = !0) {
-                            const l = f || Date.now();
+                        _innerWrite(v = 0, m = !0) {
+                            const l = v || Date.now();
                             for (; this._writeBuffer.length > this._bufferOffset;) {
                                 const s = this._writeBuffer[this._bufferOffset],
-                                    r = this._action(s, g);
+                                    r = this._action(s, m);
                                 if (r) {
-                                    const e = (h) => Date.now() - l >= 12 ? setTimeout(() => this._innerWrite(0, h)) : this._innerWrite(l, h);
+                                    const t = (h) => Date.now() - l >= 12 ? setTimeout(() => this._innerWrite(0, h)) : this._innerWrite(l, h);
                                     return void r.catch((h) => (queueMicrotask(() => {
                                         throw h;
-                                    }), Promise.resolve(!1))).then(e);
+                                    }), Promise.resolve(!1))).then(t);
                                 }
-                                const t = this._callbacks[this._bufferOffset];
-                                if (t && t(), this._bufferOffset++, this._pendingData -= s.length, Date.now() - l >= 12)
+                                const e = this._callbacks[this._bufferOffset];
+                                if (e && e(), this._bufferOffset++, this._pendingData -= s.length, Date.now() - l >= 12)
                                     break;
                             }
                             this._writeBuffer.length > this._bufferOffset ? (this._bufferOffset > 50 && (this._writeBuffer = this._writeBuffer.slice(this._bufferOffset), this._callbacks = this._callbacks.slice(this._bufferOffset), this._bufferOffset = 0), setTimeout(() => this._innerWrite())) : (this._writeBuffer.length = 0, this._callbacks.length = 0, this._pendingData = 0, this._bufferOffset = 0), this._onWriteParsed.fire();
                         }
                     }
                     i.WriteBuffer = a;
                 },
@@ -8857,50 +8857,50 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.toRgbString = i.parseColor = void 0;
                     const n = /^([\da-f])\/([\da-f])\/([\da-f])$|^([\da-f]{2})\/([\da-f]{2})\/([\da-f]{2})$|^([\da-f]{3})\/([\da-f]{3})\/([\da-f]{3})$|^([\da-f]{4})\/([\da-f]{4})\/([\da-f]{4})$/,
                         o = /^[\da-f]+$/;
 
                     function c(a, d) {
-                        const f = a.toString(16),
-                            g = f.length < 2 ? "0" + f : f;
+                        const v = a.toString(16),
+                            m = v.length < 2 ? "0" + v : v;
                         switch (d) {
                             case 4:
-                                return f[0];
+                                return v[0];
                             case 8:
-                                return g;
+                                return m;
                             case 12:
-                                return (g + g).slice(0, 3);
+                                return (m + m).slice(0, 3);
                             default:
-                                return g + g;
+                                return m + m;
                         }
                     }
                     i.parseColor = function(a) {
                         if (!a)
                             return;
                         let d = a.toLowerCase();
                         if (d.indexOf("rgb:") === 0) {
                             d = d.slice(4);
-                            const f = n.exec(d);
-                            if (f) {
-                                const g = f[1] ? 15 : f[4] ? 255 : f[7] ? 4095 : 65535;
-                                return [Math.round(parseInt(f[1] || f[4] || f[7] || f[10], 16) / g * 255), Math.round(parseInt(f[2] || f[5] || f[8] || f[11], 16) / g * 255), Math.round(parseInt(f[3] || f[6] || f[9] || f[12], 16) / g * 255)];
+                            const v = n.exec(d);
+                            if (v) {
+                                const m = v[1] ? 15 : v[4] ? 255 : v[7] ? 4095 : 65535;
+                                return [Math.round(parseInt(v[1] || v[4] || v[7] || v[10], 16) / m * 255), Math.round(parseInt(v[2] || v[5] || v[8] || v[11], 16) / m * 255), Math.round(parseInt(v[3] || v[6] || v[9] || v[12], 16) / m * 255)];
                             }
                         } else if (d.indexOf("#") === 0 && (d = d.slice(1), o.exec(d) && [3, 6, 9, 12].includes(d.length))) {
-                            const f = d.length / 3,
-                                g = [0, 0, 0];
+                            const v = d.length / 3,
+                                m = [0, 0, 0];
                             for (let l = 0; l < 3; ++l) {
-                                const s = parseInt(d.slice(f * l, f * l + f), 16);
-                                g[l] = f === 1 ? s << 4 : f === 2 ? s : f === 3 ? s >> 4 : s >> 8;
+                                const s = parseInt(d.slice(v * l, v * l + v), 16);
+                                m[l] = v === 1 ? s << 4 : v === 2 ? s : v === 3 ? s >> 4 : s >> 8;
                             }
-                            return g;
+                            return m;
                         }
                     }, i.toRgbString = function(a, d = 16) {
-                        const [f, g, l] = a;
-                        return `rgb:${c(f, d)}/${c(g, d)}/${c(l, d)}`;
+                        const [v, m, l] = a;
+                        return `rgb:${c(v, d)}/${c(m, d)}/${c(l, d)}`;
                     };
                 },
                 5770: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.PAYLOAD_LIMIT = void 0, i.PAYLOAD_LIMIT = 1e7;
                 },
@@ -8919,233 +8919,233 @@
                                 loopPosition: 0,
                                 fallThrough: !1
                             };
                         }
                         dispose() {
                             this._handlers = /* @__PURE__ */ Object.create(null), this._handlerFb = () => {}, this._active = d;
                         }
-                        registerHandler(g, l) {
-                            this._handlers[g] === void 0 && (this._handlers[g] = []);
-                            const s = this._handlers[g];
+                        registerHandler(m, l) {
+                            this._handlers[m] === void 0 && (this._handlers[m] = []);
+                            const s = this._handlers[m];
                             return s.push(l), {
                                 dispose: () => {
                                     const r = s.indexOf(l);
                                     r !== -1 && s.splice(r, 1);
                                 }
                             };
                         }
-                        clearHandler(g) {
-                            this._handlers[g] && delete this._handlers[g];
+                        clearHandler(m) {
+                            this._handlers[m] && delete this._handlers[m];
                         }
-                        setHandlerFallback(g) {
-                            this._handlerFb = g;
+                        setHandlerFallback(m) {
+                            this._handlerFb = m;
                         }
                         reset() {
                             if (this._active.length)
-                                for (let g = this._stack.paused ? this._stack.loopPosition - 1 : this._active.length - 1; g >= 0; --g)
-                                    this._active[g].unhook(!1);
+                                for (let m = this._stack.paused ? this._stack.loopPosition - 1 : this._active.length - 1; m >= 0; --m)
+                                    this._active[m].unhook(!1);
                             this._stack.paused = !1, this._active = d, this._ident = 0;
                         }
-                        hook(g, l) {
-                            if (this.reset(), this._ident = g, this._active = this._handlers[g] || d, this._active.length)
+                        hook(m, l) {
+                            if (this.reset(), this._ident = m, this._active = this._handlers[m] || d, this._active.length)
                                 for (let s = this._active.length - 1; s >= 0; s--)
                                     this._active[s].hook(l);
                             else
                                 this._handlerFb(this._ident, "HOOK", l);
                         }
-                        put(g, l, s) {
+                        put(m, l, s) {
                             if (this._active.length)
                                 for (let r = this._active.length - 1; r >= 0; r--)
-                                    this._active[r].put(g, l, s);
+                                    this._active[r].put(m, l, s);
                             else
-                                this._handlerFb(this._ident, "PUT", (0, o.utf32ToString)(g, l, s));
+                                this._handlerFb(this._ident, "PUT", (0, o.utf32ToString)(m, l, s));
                         }
-                        unhook(g, l = !0) {
+                        unhook(m, l = !0) {
                             if (this._active.length) {
                                 let s = !1,
                                     r = this._active.length - 1,
-                                    t = !1;
-                                if (this._stack.paused && (r = this._stack.loopPosition - 1, s = l, t = this._stack.fallThrough, this._stack.paused = !1), !t && s === !1) {
-                                    for (; r >= 0 && (s = this._active[r].unhook(g), s !== !0); r--)
+                                    e = !1;
+                                if (this._stack.paused && (r = this._stack.loopPosition - 1, s = l, e = this._stack.fallThrough, this._stack.paused = !1), !e && s === !1) {
+                                    for (; r >= 0 && (s = this._active[r].unhook(m), s !== !0); r--)
                                         if (s instanceof Promise)
                                             return this._stack.paused = !0, this._stack.loopPosition = r, this._stack.fallThrough = !1, s;
                                     r--;
                                 }
                                 for (; r >= 0; r--)
                                     if (s = this._active[r].unhook(!1), s instanceof Promise)
                                         return this._stack.paused = !0, this._stack.loopPosition = r, this._stack.fallThrough = !0, s;
                             } else
-                                this._handlerFb(this._ident, "UNHOOK", g);
+                                this._handlerFb(this._ident, "UNHOOK", m);
                             this._active = d, this._ident = 0;
                         }
                     };
-                    const f = new c.Params();
-                    f.addParam(0), i.DcsHandler = class {
-                        constructor(g) {
-                            this._handler = g, this._data = "", this._params = f, this._hitLimit = !1;
+                    const v = new c.Params();
+                    v.addParam(0), i.DcsHandler = class {
+                        constructor(m) {
+                            this._handler = m, this._data = "", this._params = v, this._hitLimit = !1;
                         }
-                        hook(g) {
-                            this._params = g.length > 1 || g.params[0] ? g.clone() : f, this._data = "", this._hitLimit = !1;
+                        hook(m) {
+                            this._params = m.length > 1 || m.params[0] ? m.clone() : v, this._data = "", this._hitLimit = !1;
                         }
-                        put(g, l, s) {
-                            this._hitLimit || (this._data += (0, o.utf32ToString)(g, l, s), this._data.length > a.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
+                        put(m, l, s) {
+                            this._hitLimit || (this._data += (0, o.utf32ToString)(m, l, s), this._data.length > a.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
                         }
-                        unhook(g) {
+                        unhook(m) {
                             let l = !1;
                             if (this._hitLimit)
                                 l = !1;
-                            else if (g && (l = this._handler(this._data, this._params), l instanceof Promise))
-                                return l.then((s) => (this._params = f, this._data = "", this._hitLimit = !1, s));
-                            return this._params = f, this._data = "", this._hitLimit = !1, l;
+                            else if (m && (l = this._handler(this._data, this._params), l instanceof Promise))
+                                return l.then((s) => (this._params = v, this._data = "", this._hitLimit = !1, s));
+                            return this._params = v, this._data = "", this._hitLimit = !1, l;
                         }
                     };
                 },
                 2015: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.EscapeSequenceParser = i.VT500_TRANSITION_TABLE = i.TransitionTable = void 0;
                     const o = n(844),
                         c = n(8742),
                         a = n(6242),
                         d = n(6351);
-                    class f {
+                    class v {
                         constructor(r) {
                             this.table = new Uint8Array(r);
                         }
-                        setDefault(r, t) {
-                            this.table.fill(r << 4 | t);
+                        setDefault(r, e) {
+                            this.table.fill(r << 4 | e);
                         }
-                        add(r, t, e, h) {
-                            this.table[t << 8 | r] = e << 4 | h;
+                        add(r, e, t, h) {
+                            this.table[e << 8 | r] = t << 4 | h;
                         }
-                        addMany(r, t, e, h) {
-                            for (let v = 0; v < r.length; v++)
-                                this.table[t << 8 | r[v]] = e << 4 | h;
+                        addMany(r, e, t, h) {
+                            for (let g = 0; g < r.length; g++)
+                                this.table[e << 8 | r[g]] = t << 4 | h;
                         }
                     }
-                    i.TransitionTable = f;
-                    const g = 160;
+                    i.TransitionTable = v;
+                    const m = 160;
                     i.VT500_TRANSITION_TABLE = function() {
-                        const s = new f(4095),
-                            r = Array.apply(null, Array(256)).map((p, _) => _),
-                            t = (p, _) => r.slice(p, _),
-                            e = t(32, 127),
-                            h = t(0, 24);
-                        h.push(25), h.push.apply(h, t(28, 32));
-                        const v = t(0, 14);
+                        const s = new v(4095),
+                            r = Array.apply(null, Array(256)).map((S, _) => _),
+                            e = (S, _) => r.slice(S, _),
+                            t = e(32, 127),
+                            h = e(0, 24);
+                        h.push(25), h.push.apply(h, e(28, 32));
+                        const g = e(0, 14);
                         let u;
-                        for (u in s.setDefault(1, 0), s.addMany(e, 0, 2, 0), v)
-                            s.addMany([24, 26, 153, 154], u, 3, 0), s.addMany(t(128, 144), u, 3, 0), s.addMany(t(144, 152), u, 3, 0), s.add(156, u, 0, 0), s.add(27, u, 11, 1), s.add(157, u, 4, 8), s.addMany([152, 158, 159], u, 0, 7), s.add(155, u, 11, 3), s.add(144, u, 11, 9);
-                        return s.addMany(h, 0, 3, 0), s.addMany(h, 1, 3, 1), s.add(127, 1, 0, 1), s.addMany(h, 8, 0, 8), s.addMany(h, 3, 3, 3), s.add(127, 3, 0, 3), s.addMany(h, 4, 3, 4), s.add(127, 4, 0, 4), s.addMany(h, 6, 3, 6), s.addMany(h, 5, 3, 5), s.add(127, 5, 0, 5), s.addMany(h, 2, 3, 2), s.add(127, 2, 0, 2), s.add(93, 1, 4, 8), s.addMany(e, 8, 5, 8), s.add(127, 8, 5, 8), s.addMany([156, 27, 24, 26, 7], 8, 6, 0), s.addMany(t(28, 32), 8, 0, 8), s.addMany([88, 94, 95], 1, 0, 7), s.addMany(e, 7, 0, 7), s.addMany(h, 7, 0, 7), s.add(156, 7, 0, 0), s.add(127, 7, 0, 7), s.add(91, 1, 11, 3), s.addMany(t(64, 127), 3, 7, 0), s.addMany(t(48, 60), 3, 8, 4), s.addMany([60, 61, 62, 63], 3, 9, 4), s.addMany(t(48, 60), 4, 8, 4), s.addMany(t(64, 127), 4, 7, 0), s.addMany([60, 61, 62, 63], 4, 0, 6), s.addMany(t(32, 64), 6, 0, 6), s.add(127, 6, 0, 6), s.addMany(t(64, 127), 6, 0, 0), s.addMany(t(32, 48), 3, 9, 5), s.addMany(t(32, 48), 5, 9, 5), s.addMany(t(48, 64), 5, 0, 6), s.addMany(t(64, 127), 5, 7, 0), s.addMany(t(32, 48), 4, 9, 5), s.addMany(t(32, 48), 1, 9, 2), s.addMany(t(32, 48), 2, 9, 2), s.addMany(t(48, 127), 2, 10, 0), s.addMany(t(48, 80), 1, 10, 0), s.addMany(t(81, 88), 1, 10, 0), s.addMany([89, 90, 92], 1, 10, 0), s.addMany(t(96, 127), 1, 10, 0), s.add(80, 1, 11, 9), s.addMany(h, 9, 0, 9), s.add(127, 9, 0, 9), s.addMany(t(28, 32), 9, 0, 9), s.addMany(t(32, 48), 9, 9, 12), s.addMany(t(48, 60), 9, 8, 10), s.addMany([60, 61, 62, 63], 9, 9, 10), s.addMany(h, 11, 0, 11), s.addMany(t(32, 128), 11, 0, 11), s.addMany(t(28, 32), 11, 0, 11), s.addMany(h, 10, 0, 10), s.add(127, 10, 0, 10), s.addMany(t(28, 32), 10, 0, 10), s.addMany(t(48, 60), 10, 8, 10), s.addMany([60, 61, 62, 63], 10, 0, 11), s.addMany(t(32, 48), 10, 9, 12), s.addMany(h, 12, 0, 12), s.add(127, 12, 0, 12), s.addMany(t(28, 32), 12, 0, 12), s.addMany(t(32, 48), 12, 9, 12), s.addMany(t(48, 64), 12, 0, 11), s.addMany(t(64, 127), 12, 12, 13), s.addMany(t(64, 127), 10, 12, 13), s.addMany(t(64, 127), 9, 12, 13), s.addMany(h, 13, 13, 13), s.addMany(e, 13, 13, 13), s.add(127, 13, 0, 13), s.addMany([27, 156, 24, 26], 13, 14, 0), s.add(g, 0, 2, 0), s.add(g, 8, 5, 8), s.add(g, 6, 0, 6), s.add(g, 11, 0, 11), s.add(g, 13, 13, 13), s;
+                        for (u in s.setDefault(1, 0), s.addMany(t, 0, 2, 0), g)
+                            s.addMany([24, 26, 153, 154], u, 3, 0), s.addMany(e(128, 144), u, 3, 0), s.addMany(e(144, 152), u, 3, 0), s.add(156, u, 0, 0), s.add(27, u, 11, 1), s.add(157, u, 4, 8), s.addMany([152, 158, 159], u, 0, 7), s.add(155, u, 11, 3), s.add(144, u, 11, 9);
+                        return s.addMany(h, 0, 3, 0), s.addMany(h, 1, 3, 1), s.add(127, 1, 0, 1), s.addMany(h, 8, 0, 8), s.addMany(h, 3, 3, 3), s.add(127, 3, 0, 3), s.addMany(h, 4, 3, 4), s.add(127, 4, 0, 4), s.addMany(h, 6, 3, 6), s.addMany(h, 5, 3, 5), s.add(127, 5, 0, 5), s.addMany(h, 2, 3, 2), s.add(127, 2, 0, 2), s.add(93, 1, 4, 8), s.addMany(t, 8, 5, 8), s.add(127, 8, 5, 8), s.addMany([156, 27, 24, 26, 7], 8, 6, 0), s.addMany(e(28, 32), 8, 0, 8), s.addMany([88, 94, 95], 1, 0, 7), s.addMany(t, 7, 0, 7), s.addMany(h, 7, 0, 7), s.add(156, 7, 0, 0), s.add(127, 7, 0, 7), s.add(91, 1, 11, 3), s.addMany(e(64, 127), 3, 7, 0), s.addMany(e(48, 60), 3, 8, 4), s.addMany([60, 61, 62, 63], 3, 9, 4), s.addMany(e(48, 60), 4, 8, 4), s.addMany(e(64, 127), 4, 7, 0), s.addMany([60, 61, 62, 63], 4, 0, 6), s.addMany(e(32, 64), 6, 0, 6), s.add(127, 6, 0, 6), s.addMany(e(64, 127), 6, 0, 0), s.addMany(e(32, 48), 3, 9, 5), s.addMany(e(32, 48), 5, 9, 5), s.addMany(e(48, 64), 5, 0, 6), s.addMany(e(64, 127), 5, 7, 0), s.addMany(e(32, 48), 4, 9, 5), s.addMany(e(32, 48), 1, 9, 2), s.addMany(e(32, 48), 2, 9, 2), s.addMany(e(48, 127), 2, 10, 0), s.addMany(e(48, 80), 1, 10, 0), s.addMany(e(81, 88), 1, 10, 0), s.addMany([89, 90, 92], 1, 10, 0), s.addMany(e(96, 127), 1, 10, 0), s.add(80, 1, 11, 9), s.addMany(h, 9, 0, 9), s.add(127, 9, 0, 9), s.addMany(e(28, 32), 9, 0, 9), s.addMany(e(32, 48), 9, 9, 12), s.addMany(e(48, 60), 9, 8, 10), s.addMany([60, 61, 62, 63], 9, 9, 10), s.addMany(h, 11, 0, 11), s.addMany(e(32, 128), 11, 0, 11), s.addMany(e(28, 32), 11, 0, 11), s.addMany(h, 10, 0, 10), s.add(127, 10, 0, 10), s.addMany(e(28, 32), 10, 0, 10), s.addMany(e(48, 60), 10, 8, 10), s.addMany([60, 61, 62, 63], 10, 0, 11), s.addMany(e(32, 48), 10, 9, 12), s.addMany(h, 12, 0, 12), s.add(127, 12, 0, 12), s.addMany(e(28, 32), 12, 0, 12), s.addMany(e(32, 48), 12, 9, 12), s.addMany(e(48, 64), 12, 0, 11), s.addMany(e(64, 127), 12, 12, 13), s.addMany(e(64, 127), 10, 12, 13), s.addMany(e(64, 127), 9, 12, 13), s.addMany(h, 13, 13, 13), s.addMany(t, 13, 13, 13), s.add(127, 13, 0, 13), s.addMany([27, 156, 24, 26], 13, 14, 0), s.add(m, 0, 2, 0), s.add(m, 8, 5, 8), s.add(m, 6, 0, 6), s.add(m, 11, 0, 11), s.add(m, 13, 13, 13), s;
                     }();
                     class l extends o.Disposable {
                         constructor(r = i.VT500_TRANSITION_TABLE) {
                             super(), this._transitions = r, this._parseStack = {
                                 state: 0,
                                 handlers: [],
                                 handlerPos: 0,
                                 transition: 0,
                                 chunkPos: 0
-                            }, this.initialState = 0, this.currentState = this.initialState, this._params = new c.Params(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0, this._printHandlerFb = (t, e, h) => {}, this._executeHandlerFb = (t) => {}, this._csiHandlerFb = (t, e) => {}, this._escHandlerFb = (t) => {}, this._errorHandlerFb = (t) => t, this._printHandler = this._printHandlerFb, this._executeHandlers = /* @__PURE__ */ Object.create(null), this._csiHandlers = /* @__PURE__ */ Object.create(null), this._escHandlers = /* @__PURE__ */ Object.create(null), this.register((0, o.toDisposable)(() => {
+                            }, this.initialState = 0, this.currentState = this.initialState, this._params = new c.Params(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0, this._printHandlerFb = (e, t, h) => {}, this._executeHandlerFb = (e) => {}, this._csiHandlerFb = (e, t) => {}, this._escHandlerFb = (e) => {}, this._errorHandlerFb = (e) => e, this._printHandler = this._printHandlerFb, this._executeHandlers = /* @__PURE__ */ Object.create(null), this._csiHandlers = /* @__PURE__ */ Object.create(null), this._escHandlers = /* @__PURE__ */ Object.create(null), this.register((0, o.toDisposable)(() => {
                                 this._csiHandlers = /* @__PURE__ */ Object.create(null), this._executeHandlers = /* @__PURE__ */ Object.create(null), this._escHandlers = /* @__PURE__ */ Object.create(null);
                             })), this._oscParser = this.register(new a.OscParser()), this._dcsParser = this.register(new d.DcsParser()), this._errorHandler = this._errorHandlerFb, this.registerEscHandler({
                                 final: "\\"
                             }, () => !0);
                         }
-                        _identifier(r, t = [64, 126]) {
-                            let e = 0;
+                        _identifier(r, e = [64, 126]) {
+                            let t = 0;
                             if (r.prefix) {
                                 if (r.prefix.length > 1)
                                     throw new Error("only one byte as prefix supported");
-                                if (e = r.prefix.charCodeAt(0), e && 60 > e || e > 63)
+                                if (t = r.prefix.charCodeAt(0), t && 60 > t || t > 63)
                                     throw new Error("prefix must be in range 0x3c .. 0x3f");
                             }
                             if (r.intermediates) {
                                 if (r.intermediates.length > 2)
                                     throw new Error("only two bytes as intermediates are supported");
-                                for (let v = 0; v < r.intermediates.length; ++v) {
-                                    const u = r.intermediates.charCodeAt(v);
+                                for (let g = 0; g < r.intermediates.length; ++g) {
+                                    const u = r.intermediates.charCodeAt(g);
                                     if (32 > u || u > 47)
                                         throw new Error("intermediate must be in range 0x20 .. 0x2f");
-                                    e <<= 8, e |= u;
+                                    t <<= 8, t |= u;
                                 }
                             }
                             if (r.final.length !== 1)
                                 throw new Error("final must be a single byte");
                             const h = r.final.charCodeAt(0);
-                            if (t[0] > h || h > t[1])
-                                throw new Error(`final must be in range ${t[0]} .. ${t[1]}`);
-                            return e <<= 8, e |= h, e;
+                            if (e[0] > h || h > e[1])
+                                throw new Error(`final must be in range ${e[0]} .. ${e[1]}`);
+                            return t <<= 8, t |= h, t;
                         }
                         identToString(r) {
-                            const t = [];
+                            const e = [];
                             for (; r;)
-                                t.push(String.fromCharCode(255 & r)), r >>= 8;
-                            return t.reverse().join("");
+                                e.push(String.fromCharCode(255 & r)), r >>= 8;
+                            return e.reverse().join("");
                         }
                         setPrintHandler(r) {
                             this._printHandler = r;
                         }
                         clearPrintHandler() {
                             this._printHandler = this._printHandlerFb;
                         }
-                        registerEscHandler(r, t) {
-                            const e = this._identifier(r, [48, 126]);
-                            this._escHandlers[e] === void 0 && (this._escHandlers[e] = []);
-                            const h = this._escHandlers[e];
-                            return h.push(t), {
+                        registerEscHandler(r, e) {
+                            const t = this._identifier(r, [48, 126]);
+                            this._escHandlers[t] === void 0 && (this._escHandlers[t] = []);
+                            const h = this._escHandlers[t];
+                            return h.push(e), {
                                 dispose: () => {
-                                    const v = h.indexOf(t);
-                                    v !== -1 && h.splice(v, 1);
+                                    const g = h.indexOf(e);
+                                    g !== -1 && h.splice(g, 1);
                                 }
                             };
                         }
                         clearEscHandler(r) {
                             this._escHandlers[this._identifier(r, [48, 126])] && delete this._escHandlers[this._identifier(r, [48, 126])];
                         }
                         setEscHandlerFallback(r) {
                             this._escHandlerFb = r;
                         }
-                        setExecuteHandler(r, t) {
-                            this._executeHandlers[r.charCodeAt(0)] = t;
+                        setExecuteHandler(r, e) {
+                            this._executeHandlers[r.charCodeAt(0)] = e;
                         }
                         clearExecuteHandler(r) {
                             this._executeHandlers[r.charCodeAt(0)] && delete this._executeHandlers[r.charCodeAt(0)];
                         }
                         setExecuteHandlerFallback(r) {
                             this._executeHandlerFb = r;
                         }
-                        registerCsiHandler(r, t) {
-                            const e = this._identifier(r);
-                            this._csiHandlers[e] === void 0 && (this._csiHandlers[e] = []);
-                            const h = this._csiHandlers[e];
-                            return h.push(t), {
+                        registerCsiHandler(r, e) {
+                            const t = this._identifier(r);
+                            this._csiHandlers[t] === void 0 && (this._csiHandlers[t] = []);
+                            const h = this._csiHandlers[t];
+                            return h.push(e), {
                                 dispose: () => {
-                                    const v = h.indexOf(t);
-                                    v !== -1 && h.splice(v, 1);
+                                    const g = h.indexOf(e);
+                                    g !== -1 && h.splice(g, 1);
                                 }
                             };
                         }
                         clearCsiHandler(r) {
                             this._csiHandlers[this._identifier(r)] && delete this._csiHandlers[this._identifier(r)];
                         }
                         setCsiHandlerFallback(r) {
                             this._csiHandlerFb = r;
                         }
-                        registerDcsHandler(r, t) {
-                            return this._dcsParser.registerHandler(this._identifier(r), t);
+                        registerDcsHandler(r, e) {
+                            return this._dcsParser.registerHandler(this._identifier(r), e);
                         }
                         clearDcsHandler(r) {
                             this._dcsParser.clearHandler(this._identifier(r));
                         }
                         setDcsHandlerFallback(r) {
                             this._dcsParser.setHandlerFallback(r);
                         }
-                        registerOscHandler(r, t) {
-                            return this._oscParser.registerHandler(r, t);
+                        registerOscHandler(r, e) {
+                            return this._oscParser.registerHandler(r, e);
                         }
                         clearOscHandler(r) {
                             this._oscParser.clearHandler(r);
                         }
                         setOscHandlerFallback(r) {
                             this._oscParser.setHandlerFallback(r);
                         }
@@ -9154,162 +9154,162 @@
                         }
                         clearErrorHandler() {
                             this._errorHandler = this._errorHandlerFb;
                         }
                         reset() {
                             this.currentState = this.initialState, this._oscParser.reset(), this._dcsParser.reset(), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0, this._parseStack.state !== 0 && (this._parseStack.state = 2, this._parseStack.handlers = []);
                         }
-                        _preserveStack(r, t, e, h, v) {
-                            this._parseStack.state = r, this._parseStack.handlers = t, this._parseStack.handlerPos = e, this._parseStack.transition = h, this._parseStack.chunkPos = v;
+                        _preserveStack(r, e, t, h, g) {
+                            this._parseStack.state = r, this._parseStack.handlers = e, this._parseStack.handlerPos = t, this._parseStack.transition = h, this._parseStack.chunkPos = g;
                         }
-                        parse(r, t, e) {
-                            let h, v = 0,
+                        parse(r, e, t) {
+                            let h, g = 0,
                                 u = 0,
-                                p = 0;
+                                S = 0;
                             if (this._parseStack.state)
                                 if (this._parseStack.state === 2)
-                                    this._parseStack.state = 0, p = this._parseStack.chunkPos + 1;
+                                    this._parseStack.state = 0, S = this._parseStack.chunkPos + 1;
                                 else {
-                                    if (e === void 0 || this._parseStack.state === 1)
+                                    if (t === void 0 || this._parseStack.state === 1)
                                         throw this._parseStack.state = 1, new Error("improper continuation due to previous async handler, giving up parsing");
                                     const _ = this._parseStack.handlers;
                                     let b = this._parseStack.handlerPos - 1;
                                     switch (this._parseStack.state) {
                                         case 3:
-                                            if (e === !1 && b > -1) {
+                                            if (t === !1 && b > -1) {
                                                 for (; b >= 0 && (h = _[b](this._params), h !== !0); b--)
                                                     if (h instanceof Promise)
                                                         return this._parseStack.handlerPos = b, h;
                                             }
                                             this._parseStack.handlers = [];
                                             break;
                                         case 4:
-                                            if (e === !1 && b > -1) {
+                                            if (t === !1 && b > -1) {
                                                 for (; b >= 0 && (h = _[b](), h !== !0); b--)
                                                     if (h instanceof Promise)
                                                         return this._parseStack.handlerPos = b, h;
                                             }
                                             this._parseStack.handlers = [];
                                             break;
                                         case 6:
-                                            if (v = r[this._parseStack.chunkPos], h = this._dcsParser.unhook(v !== 24 && v !== 26, e), h)
+                                            if (g = r[this._parseStack.chunkPos], h = this._dcsParser.unhook(g !== 24 && g !== 26, t), h)
                                                 return h;
-                                            v === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0;
+                                            g === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0;
                                             break;
                                         case 5:
-                                            if (v = r[this._parseStack.chunkPos], h = this._oscParser.end(v !== 24 && v !== 26, e), h)
+                                            if (g = r[this._parseStack.chunkPos], h = this._oscParser.end(g !== 24 && g !== 26, t), h)
                                                 return h;
-                                            v === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0;
+                                            g === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0;
                                     }
-                                    this._parseStack.state = 0, p = this._parseStack.chunkPos + 1, this.precedingJoinState = 0, this.currentState = 15 & this._parseStack.transition;
+                                    this._parseStack.state = 0, S = this._parseStack.chunkPos + 1, this.precedingJoinState = 0, this.currentState = 15 & this._parseStack.transition;
                                 }
-                            for (let _ = p; _ < t; ++_) {
-                                switch (v = r[_], u = this._transitions.table[this.currentState << 8 | (v < 160 ? v : g)], u >> 4) {
+                            for (let _ = S; _ < e; ++_) {
+                                switch (g = r[_], u = this._transitions.table[this.currentState << 8 | (g < 160 ? g : m)], u >> 4) {
                                     case 2:
                                         for (let L = _ + 1;; ++L) {
-                                            if (L >= t || (v = r[L]) < 32 || v > 126 && v < g) {
+                                            if (L >= e || (g = r[L]) < 32 || g > 126 && g < m) {
                                                 this._printHandler(r, _, L), _ = L - 1;
                                                 break;
                                             }
-                                            if (++L >= t || (v = r[L]) < 32 || v > 126 && v < g) {
+                                            if (++L >= e || (g = r[L]) < 32 || g > 126 && g < m) {
                                                 this._printHandler(r, _, L), _ = L - 1;
                                                 break;
                                             }
-                                            if (++L >= t || (v = r[L]) < 32 || v > 126 && v < g) {
+                                            if (++L >= e || (g = r[L]) < 32 || g > 126 && g < m) {
                                                 this._printHandler(r, _, L), _ = L - 1;
                                                 break;
                                             }
-                                            if (++L >= t || (v = r[L]) < 32 || v > 126 && v < g) {
+                                            if (++L >= e || (g = r[L]) < 32 || g > 126 && g < m) {
                                                 this._printHandler(r, _, L), _ = L - 1;
                                                 break;
                                             }
                                         }
                                         break;
                                     case 3:
-                                        this._executeHandlers[v] ? this._executeHandlers[v]() : this._executeHandlerFb(v), this.precedingJoinState = 0;
+                                        this._executeHandlers[g] ? this._executeHandlers[g]() : this._executeHandlerFb(g), this.precedingJoinState = 0;
                                         break;
                                     case 0:
                                         break;
                                     case 1:
                                         if (this._errorHandler({
                                                 position: _,
-                                                code: v,
+                                                code: g,
                                                 currentState: this.currentState,
                                                 collect: this._collect,
                                                 params: this._params,
                                                 abort: !1
                                             }).abort)
                                             return;
                                         break;
                                     case 7:
-                                        const b = this._csiHandlers[this._collect << 8 | v];
-                                        let A = b ? b.length - 1 : -1;
-                                        for (; A >= 0 && (h = b[A](this._params), h !== !0); A--)
+                                        const b = this._csiHandlers[this._collect << 8 | g];
+                                        let R = b ? b.length - 1 : -1;
+                                        for (; R >= 0 && (h = b[R](this._params), h !== !0); R--)
                                             if (h instanceof Promise)
-                                                return this._preserveStack(3, b, A, u, _), h;
-                                        A < 0 && this._csiHandlerFb(this._collect << 8 | v, this._params), this.precedingJoinState = 0;
+                                                return this._preserveStack(3, b, R, u, _), h;
+                                        R < 0 && this._csiHandlerFb(this._collect << 8 | g, this._params), this.precedingJoinState = 0;
                                         break;
                                     case 8:
                                         do
-                                            switch (v) {
+                                            switch (g) {
                                                 case 59:
                                                     this._params.addParam(0);
                                                     break;
                                                 case 58:
                                                     this._params.addSubParam(-1);
                                                     break;
                                                 default:
-                                                    this._params.addDigit(v - 48);
+                                                    this._params.addDigit(g - 48);
                                             }
-                                        while (++_ < t && (v = r[_]) > 47 && v < 60);
+                                        while (++_ < e && (g = r[_]) > 47 && g < 60);
                                         _--;
                                         break;
                                     case 9:
-                                        this._collect <<= 8, this._collect |= v;
+                                        this._collect <<= 8, this._collect |= g;
                                         break;
                                     case 10:
-                                        const T = this._escHandlers[this._collect << 8 | v];
-                                        let x = T ? T.length - 1 : -1;
-                                        for (; x >= 0 && (h = T[x](), h !== !0); x--)
+                                        const B = this._escHandlers[this._collect << 8 | g];
+                                        let T = B ? B.length - 1 : -1;
+                                        for (; T >= 0 && (h = B[T](), h !== !0); T--)
                                             if (h instanceof Promise)
-                                                return this._preserveStack(4, T, x, u, _), h;
-                                        x < 0 && this._escHandlerFb(this._collect << 8 | v), this.precedingJoinState = 0;
+                                                return this._preserveStack(4, B, T, u, _), h;
+                                        T < 0 && this._escHandlerFb(this._collect << 8 | g), this.precedingJoinState = 0;
                                         break;
                                     case 11:
                                         this._params.reset(), this._params.addParam(0), this._collect = 0;
                                         break;
                                     case 12:
-                                        this._dcsParser.hook(this._collect << 8 | v, this._params);
+                                        this._dcsParser.hook(this._collect << 8 | g, this._params);
                                         break;
                                     case 13:
                                         for (let L = _ + 1;; ++L)
-                                            if (L >= t || (v = r[L]) === 24 || v === 26 || v === 27 || v > 127 && v < g) {
+                                            if (L >= e || (g = r[L]) === 24 || g === 26 || g === 27 || g > 127 && g < m) {
                                                 this._dcsParser.put(r, _, L), _ = L - 1;
                                                 break;
                                             }
                                         break;
                                     case 14:
-                                        if (h = this._dcsParser.unhook(v !== 24 && v !== 26), h)
+                                        if (h = this._dcsParser.unhook(g !== 24 && g !== 26), h)
                                             return this._preserveStack(6, [], 0, u, _), h;
-                                        v === 27 && (u |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0;
+                                        g === 27 && (u |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0;
                                         break;
                                     case 4:
                                         this._oscParser.start();
                                         break;
                                     case 5:
                                         for (let L = _ + 1;; L++)
-                                            if (L >= t || (v = r[L]) < 32 || v > 127 && v < g) {
+                                            if (L >= e || (g = r[L]) < 32 || g > 127 && g < m) {
                                                 this._oscParser.put(r, _, L), _ = L - 1;
                                                 break;
                                             }
                                         break;
                                     case 6:
-                                        if (h = this._oscParser.end(v !== 24 && v !== 26), h)
+                                        if (h = this._oscParser.end(g !== 24 && g !== 26), h)
                                             return this._preserveStack(5, [], 0, u, _), h;
-                                        v === 27 && (u |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0;
+                                        g === 27 && (u |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingJoinState = 0;
                                 }
                                 this.currentState = 15 & u;
                             }
                         }
                     }
                     i.EscapeSequenceParser = l;
                 },
@@ -9324,21 +9324,21 @@
                         constructor() {
                             this._state = 0, this._active = a, this._id = -1, this._handlers = /* @__PURE__ */ Object.create(null), this._handlerFb = () => {}, this._stack = {
                                 paused: !1,
                                 loopPosition: 0,
                                 fallThrough: !1
                             };
                         }
-                        registerHandler(d, f) {
+                        registerHandler(d, v) {
                             this._handlers[d] === void 0 && (this._handlers[d] = []);
-                            const g = this._handlers[d];
-                            return g.push(f), {
+                            const m = this._handlers[d];
+                            return m.push(v), {
                                 dispose: () => {
-                                    const l = g.indexOf(f);
-                                    l !== -1 && g.splice(l, 1);
+                                    const l = m.indexOf(v);
+                                    l !== -1 && m.splice(l, 1);
                                 }
                             };
                         }
                         clearHandler(d) {
                             this._handlers[d] && delete this._handlers[d];
                         }
                         setHandlerFallback(d) {
@@ -9356,98 +9356,98 @@
                         _start() {
                             if (this._active = this._handlers[this._id] || a, this._active.length)
                                 for (let d = this._active.length - 1; d >= 0; d--)
                                     this._active[d].start();
                             else
                                 this._handlerFb(this._id, "START");
                         }
-                        _put(d, f, g) {
+                        _put(d, v, m) {
                             if (this._active.length)
                                 for (let l = this._active.length - 1; l >= 0; l--)
-                                    this._active[l].put(d, f, g);
+                                    this._active[l].put(d, v, m);
                             else
-                                this._handlerFb(this._id, "PUT", (0, c.utf32ToString)(d, f, g));
+                                this._handlerFb(this._id, "PUT", (0, c.utf32ToString)(d, v, m));
                         }
                         start() {
                             this.reset(), this._state = 1;
                         }
-                        put(d, f, g) {
+                        put(d, v, m) {
                             if (this._state !== 3) {
                                 if (this._state === 1)
-                                    for (; f < g;) {
-                                        const l = d[f++];
+                                    for (; v < m;) {
+                                        const l = d[v++];
                                         if (l === 59) {
                                             this._state = 2, this._start();
                                             break;
                                         }
                                         if (l < 48 || 57 < l)
                                             return void(this._state = 3);
                                         this._id === -1 && (this._id = 0), this._id = 10 * this._id + l - 48;
                                     }
-                                this._state === 2 && g - f > 0 && this._put(d, f, g);
+                                this._state === 2 && m - v > 0 && this._put(d, v, m);
                             }
                         }
-                        end(d, f = !0) {
+                        end(d, v = !0) {
                             if (this._state !== 0) {
                                 if (this._state !== 3)
                                     if (this._state === 1 && this._start(), this._active.length) {
-                                        let g = !1,
+                                        let m = !1,
                                             l = this._active.length - 1,
                                             s = !1;
-                                        if (this._stack.paused && (l = this._stack.loopPosition - 1, g = f, s = this._stack.fallThrough, this._stack.paused = !1), !s && g === !1) {
-                                            for (; l >= 0 && (g = this._active[l].end(d), g !== !0); l--)
-                                                if (g instanceof Promise)
-                                                    return this._stack.paused = !0, this._stack.loopPosition = l, this._stack.fallThrough = !1, g;
+                                        if (this._stack.paused && (l = this._stack.loopPosition - 1, m = v, s = this._stack.fallThrough, this._stack.paused = !1), !s && m === !1) {
+                                            for (; l >= 0 && (m = this._active[l].end(d), m !== !0); l--)
+                                                if (m instanceof Promise)
+                                                    return this._stack.paused = !0, this._stack.loopPosition = l, this._stack.fallThrough = !1, m;
                                             l--;
                                         }
                                         for (; l >= 0; l--)
-                                            if (g = this._active[l].end(!1), g instanceof Promise)
-                                                return this._stack.paused = !0, this._stack.loopPosition = l, this._stack.fallThrough = !0, g;
+                                            if (m = this._active[l].end(!1), m instanceof Promise)
+                                                return this._stack.paused = !0, this._stack.loopPosition = l, this._stack.fallThrough = !0, m;
                                     } else
                                         this._handlerFb(this._id, "END", d);
                                 this._active = a, this._id = -1, this._state = 0;
                             }
                         }
                     }, i.OscHandler = class {
                         constructor(d) {
                             this._handler = d, this._data = "", this._hitLimit = !1;
                         }
                         start() {
                             this._data = "", this._hitLimit = !1;
                         }
-                        put(d, f, g) {
-                            this._hitLimit || (this._data += (0, c.utf32ToString)(d, f, g), this._data.length > o.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
+                        put(d, v, m) {
+                            this._hitLimit || (this._data += (0, c.utf32ToString)(d, v, m), this._data.length > o.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
                         }
                         end(d) {
-                            let f = !1;
+                            let v = !1;
                             if (this._hitLimit)
-                                f = !1;
-                            else if (d && (f = this._handler(this._data), f instanceof Promise))
-                                return f.then((g) => (this._data = "", this._hitLimit = !1, g));
-                            return this._data = "", this._hitLimit = !1, f;
+                                v = !1;
+                            else if (d && (v = this._handler(this._data), v instanceof Promise))
+                                return v.then((m) => (this._data = "", this._hitLimit = !1, m));
+                            return this._data = "", this._hitLimit = !1, v;
                         }
                     };
                 },
                 8742: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.Params = void 0;
                     const n = 2147483647;
                     class o {
                         static fromArray(a) {
                             const d = new o();
                             if (!a.length)
                                 return d;
-                            for (let f = Array.isArray(a[0]) ? 1 : 0; f < a.length; ++f) {
-                                const g = a[f];
-                                if (Array.isArray(g))
-                                    for (let l = 0; l < g.length; ++l)
-                                        d.addSubParam(g[l]);
+                            for (let v = Array.isArray(a[0]) ? 1 : 0; v < a.length; ++v) {
+                                const m = a[v];
+                                if (Array.isArray(m))
+                                    for (let l = 0; l < m.length; ++l)
+                                        d.addSubParam(m[l]);
                                 else
-                                    d.addParam(g);
+                                    d.addParam(m);
                             }
                             return d;
                         }
                         constructor(a = 32, d = 32) {
                             if (this.maxLength = a, this.maxSubParamsLength = d, d > 256)
                                 throw new Error("maxSubParamsLength must not be greater than 256");
                             this.params = new Int32Array(a), this.length = 0, this._subParams = new Int32Array(d), this._subParamsLength = 0, this._subParamsIdx = new Uint16Array(a), this._rejectDigits = !1, this._rejectSubDigits = !1, this._digitIsSub = !1;
@@ -9456,17 +9456,17 @@
                             const a = new o(this.maxLength, this.maxSubParamsLength);
                             return a.params.set(this.params), a.length = this.length, a._subParams.set(this._subParams), a._subParamsLength = this._subParamsLength, a._subParamsIdx.set(this._subParamsIdx), a._rejectDigits = this._rejectDigits, a._rejectSubDigits = this._rejectSubDigits, a._digitIsSub = this._digitIsSub, a;
                         }
                         toArray() {
                             const a = [];
                             for (let d = 0; d < this.length; ++d) {
                                 a.push(this.params[d]);
-                                const f = this._subParamsIdx[d] >> 8,
-                                    g = 255 & this._subParamsIdx[d];
-                                g - f > 0 && a.push(Array.prototype.slice.call(this._subParams, f, g));
+                                const v = this._subParamsIdx[d] >> 8,
+                                    m = 255 & this._subParamsIdx[d];
+                                m - v > 0 && a.push(Array.prototype.slice.call(this._subParams, v, m));
                             }
                             return a;
                         }
                         reset() {
                             this.length = 0, this._subParamsLength = 0, this._rejectDigits = !1, this._rejectSubDigits = !1, this._digitIsSub = !1;
                         }
                         addParam(a) {
@@ -9489,33 +9489,33 @@
                                 }
                         }
                         hasSubParams(a) {
                             return (255 & this._subParamsIdx[a]) - (this._subParamsIdx[a] >> 8) > 0;
                         }
                         getSubParams(a) {
                             const d = this._subParamsIdx[a] >> 8,
-                                f = 255 & this._subParamsIdx[a];
-                            return f - d > 0 ? this._subParams.subarray(d, f) : null;
+                                v = 255 & this._subParamsIdx[a];
+                            return v - d > 0 ? this._subParams.subarray(d, v) : null;
                         }
                         getSubParamsAll() {
                             const a = {};
                             for (let d = 0; d < this.length; ++d) {
-                                const f = this._subParamsIdx[d] >> 8,
-                                    g = 255 & this._subParamsIdx[d];
-                                g - f > 0 && (a[d] = this._subParams.slice(f, g));
+                                const v = this._subParamsIdx[d] >> 8,
+                                    m = 255 & this._subParamsIdx[d];
+                                m - v > 0 && (a[d] = this._subParams.slice(v, m));
                             }
                             return a;
                         }
                         addDigit(a) {
                             let d;
                             if (this._rejectDigits || !(d = this._digitIsSub ? this._subParamsLength : this.length) || this._digitIsSub && this._rejectSubDigits)
                                 return;
-                            const f = this._digitIsSub ? this._subParams : this.params,
-                                g = f[d - 1];
-                            f[d - 1] = ~g ? Math.min(10 * g + a, n) : a;
+                            const v = this._digitIsSub ? this._subParams : this.params,
+                                m = v[d - 1];
+                            v[d - 1] = ~m ? Math.min(10 * m + a, n) : a;
                         }
                     }
                     i.Params = o;
                 },
                 5741: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
@@ -9616,16 +9616,16 @@
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.BufferNamespaceApi = void 0;
                     const o = n(8771),
                         c = n(8460),
                         a = n(844);
                     class d extends a.Disposable {
-                        constructor(g) {
-                            super(), this._core = g, this._onBufferChange = this.register(new c.EventEmitter()), this.onBufferChange = this._onBufferChange.event, this._normal = new o.BufferApiView(this._core.buffers.normal, "normal"), this._alternate = new o.BufferApiView(this._core.buffers.alt, "alternate"), this._core.buffers.onBufferActivate(() => this._onBufferChange.fire(this.active));
+                        constructor(m) {
+                            super(), this._core = m, this._onBufferChange = this.register(new c.EventEmitter()), this.onBufferChange = this._onBufferChange.event, this._normal = new o.BufferApiView(this._core.buffers.normal, "normal"), this._alternate = new o.BufferApiView(this._core.buffers.alt, "alternate"), this._core.buffers.onBufferActivate(() => this._onBufferChange.fire(this.active));
                         }
                         get active() {
                             if (this._core.buffers.active === this._core.buffers.normal)
                                 return this.normal;
                             if (this._core.buffers.active === this._core.buffers.alt)
                                 return this.alternate;
                             throw new Error("Active buffer is neither normal nor alternate");
@@ -9690,81 +9690,81 @@
                         }
                         set activeVersion(n) {
                             this._core.unicodeService.activeVersion = n;
                         }
                     };
                 },
                 744: function(k, i, n) {
-                    var o = this && this.__decorate || function(s, r, t, e) {
-                            var h, v = arguments.length,
-                                u = v < 3 ? r : e === null ? e = Object.getOwnPropertyDescriptor(r, t) : e;
+                    var o = this && this.__decorate || function(s, r, e, t) {
+                            var h, g = arguments.length,
+                                u = g < 3 ? r : t === null ? t = Object.getOwnPropertyDescriptor(r, e) : t;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                u = Reflect.decorate(s, r, t, e);
+                                u = Reflect.decorate(s, r, e, t);
                             else
-                                for (var p = s.length - 1; p >= 0; p--)
-                                    (h = s[p]) && (u = (v < 3 ? h(u) : v > 3 ? h(r, t, u) : h(r, t)) || u);
-                            return v > 3 && u && Object.defineProperty(r, t, u), u;
+                                for (var S = s.length - 1; S >= 0; S--)
+                                    (h = s[S]) && (u = (g < 3 ? h(u) : g > 3 ? h(r, e, u) : h(r, e)) || u);
+                            return g > 3 && u && Object.defineProperty(r, e, u), u;
                         },
                         c = this && this.__param || function(s, r) {
-                            return function(t, e) {
-                                r(t, e, s);
+                            return function(e, t) {
+                                r(e, t, s);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.BufferService = i.MINIMUM_ROWS = i.MINIMUM_COLS = void 0;
                     const a = n(8460),
                         d = n(844),
-                        f = n(5295),
-                        g = n(2585);
+                        v = n(5295),
+                        m = n(2585);
                     i.MINIMUM_COLS = 2, i.MINIMUM_ROWS = 1;
                     let l = i.BufferService = class extends d.Disposable {
                         get buffer() {
                             return this.buffers.active;
                         }
                         constructor(s) {
-                            super(), this.isUserScrolling = !1, this._onResize = this.register(new a.EventEmitter()), this.onResize = this._onResize.event, this._onScroll = this.register(new a.EventEmitter()), this.onScroll = this._onScroll.event, this.cols = Math.max(s.rawOptions.cols || 0, i.MINIMUM_COLS), this.rows = Math.max(s.rawOptions.rows || 0, i.MINIMUM_ROWS), this.buffers = this.register(new f.BufferSet(s, this));
+                            super(), this.isUserScrolling = !1, this._onResize = this.register(new a.EventEmitter()), this.onResize = this._onResize.event, this._onScroll = this.register(new a.EventEmitter()), this.onScroll = this._onScroll.event, this.cols = Math.max(s.rawOptions.cols || 0, i.MINIMUM_COLS), this.rows = Math.max(s.rawOptions.rows || 0, i.MINIMUM_ROWS), this.buffers = this.register(new v.BufferSet(s, this));
                         }
                         resize(s, r) {
                             this.cols = s, this.rows = r, this.buffers.resize(s, r), this._onResize.fire({
                                 cols: s,
                                 rows: r
                             });
                         }
                         reset() {
                             this.buffers.reset(), this.isUserScrolling = !1;
                         }
                         scroll(s, r = !1) {
-                            const t = this.buffer;
-                            let e;
-                            e = this._cachedBlankLine, e && e.length === this.cols && e.getFg(0) === s.fg && e.getBg(0) === s.bg || (e = t.getBlankLine(s, r), this._cachedBlankLine = e), e.isWrapped = r;
-                            const h = t.ybase + t.scrollTop,
-                                v = t.ybase + t.scrollBottom;
-                            if (t.scrollTop === 0) {
-                                const u = t.lines.isFull;
-                                v === t.lines.length - 1 ? u ? t.lines.recycle().copyFrom(e) : t.lines.push(e.clone()) : t.lines.splice(v + 1, 0, e.clone()), u ? this.isUserScrolling && (t.ydisp = Math.max(t.ydisp - 1, 0)) : (t.ybase++, this.isUserScrolling || t.ydisp++);
+                            const e = this.buffer;
+                            let t;
+                            t = this._cachedBlankLine, t && t.length === this.cols && t.getFg(0) === s.fg && t.getBg(0) === s.bg || (t = e.getBlankLine(s, r), this._cachedBlankLine = t), t.isWrapped = r;
+                            const h = e.ybase + e.scrollTop,
+                                g = e.ybase + e.scrollBottom;
+                            if (e.scrollTop === 0) {
+                                const u = e.lines.isFull;
+                                g === e.lines.length - 1 ? u ? e.lines.recycle().copyFrom(t) : e.lines.push(t.clone()) : e.lines.splice(g + 1, 0, t.clone()), u ? this.isUserScrolling && (e.ydisp = Math.max(e.ydisp - 1, 0)) : (e.ybase++, this.isUserScrolling || e.ydisp++);
                             } else {
-                                const u = v - h + 1;
-                                t.lines.shiftElements(h + 1, u - 1, -1), t.lines.set(v, e.clone());
+                                const u = g - h + 1;
+                                e.lines.shiftElements(h + 1, u - 1, -1), e.lines.set(g, t.clone());
                             }
-                            this.isUserScrolling || (t.ydisp = t.ybase), this._onScroll.fire(t.ydisp);
+                            this.isUserScrolling || (e.ydisp = e.ybase), this._onScroll.fire(e.ydisp);
                         }
-                        scrollLines(s, r, t) {
-                            const e = this.buffer;
+                        scrollLines(s, r, e) {
+                            const t = this.buffer;
                             if (s < 0) {
-                                if (e.ydisp === 0)
+                                if (t.ydisp === 0)
                                     return;
                                 this.isUserScrolling = !0;
                             } else
-                                s + e.ydisp >= e.ybase && (this.isUserScrolling = !1);
-                            const h = e.ydisp;
-                            e.ydisp = Math.max(Math.min(e.ydisp + s, e.ybase), 0), h !== e.ydisp && (r || this._onScroll.fire(e.ydisp));
+                                s + t.ydisp >= t.ybase && (this.isUserScrolling = !1);
+                            const h = t.ydisp;
+                            t.ydisp = Math.max(Math.min(t.ydisp + s, t.ybase), 0), h !== t.ydisp && (r || this._onScroll.fire(t.ydisp));
                         }
                     };
-                    i.BufferService = l = o([c(0, g.IOptionsService)], l);
+                    i.BufferService = l = o([c(0, m.IOptionsService)], l);
                 },
                 7994: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CharsetService = void 0, i.CharsetService = class {
                         constructor() {
                             this.glevel = 0, this._charsets = [];
@@ -9777,391 +9777,391 @@
                         }
                         setgCharset(n, o) {
                             this._charsets[n] = o, this.glevel === n && (this.charset = o);
                         }
                     };
                 },
                 1753: function(k, i, n) {
-                    var o = this && this.__decorate || function(e, h, v, u) {
-                            var p, _ = arguments.length,
-                                b = _ < 3 ? h : u === null ? u = Object.getOwnPropertyDescriptor(h, v) : u;
+                    var o = this && this.__decorate || function(t, h, g, u) {
+                            var S, _ = arguments.length,
+                                b = _ < 3 ? h : u === null ? u = Object.getOwnPropertyDescriptor(h, g) : u;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                b = Reflect.decorate(e, h, v, u);
+                                b = Reflect.decorate(t, h, g, u);
                             else
-                                for (var A = e.length - 1; A >= 0; A--)
-                                    (p = e[A]) && (b = (_ < 3 ? p(b) : _ > 3 ? p(h, v, b) : p(h, v)) || b);
-                            return _ > 3 && b && Object.defineProperty(h, v, b), b;
+                                for (var R = t.length - 1; R >= 0; R--)
+                                    (S = t[R]) && (b = (_ < 3 ? S(b) : _ > 3 ? S(h, g, b) : S(h, g)) || b);
+                            return _ > 3 && b && Object.defineProperty(h, g, b), b;
                         },
-                        c = this && this.__param || function(e, h) {
-                            return function(v, u) {
-                                h(v, u, e);
+                        c = this && this.__param || function(t, h) {
+                            return function(g, u) {
+                                h(g, u, t);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CoreMouseService = void 0;
                     const a = n(2585),
                         d = n(8460),
-                        f = n(844),
-                        g = {
+                        v = n(844),
+                        m = {
                             NONE: {
                                 events: 0,
                                 restrict: () => !1
                             },
                             X10: {
                                 events: 1,
-                                restrict: (e) => e.button !== 4 && e.action === 1 && (e.ctrl = !1, e.alt = !1, e.shift = !1, !0)
+                                restrict: (t) => t.button !== 4 && t.action === 1 && (t.ctrl = !1, t.alt = !1, t.shift = !1, !0)
                             },
                             VT200: {
                                 events: 19,
-                                restrict: (e) => e.action !== 32
+                                restrict: (t) => t.action !== 32
                             },
                             DRAG: {
                                 events: 23,
-                                restrict: (e) => e.action !== 32 || e.button !== 3
+                                restrict: (t) => t.action !== 32 || t.button !== 3
                             },
                             ANY: {
                                 events: 31,
-                                restrict: (e) => !0
+                                restrict: (t) => !0
                             }
                         };
 
-                    function l(e, h) {
-                        let v = (e.ctrl ? 16 : 0) | (e.shift ? 4 : 0) | (e.alt ? 8 : 0);
-                        return e.button === 4 ? (v |= 64, v |= e.action) : (v |= 3 & e.button, 4 & e.button && (v |= 64), 8 & e.button && (v |= 128), e.action === 32 ? v |= 32 : e.action !== 0 || h || (v |= 3)), v;
+                    function l(t, h) {
+                        let g = (t.ctrl ? 16 : 0) | (t.shift ? 4 : 0) | (t.alt ? 8 : 0);
+                        return t.button === 4 ? (g |= 64, g |= t.action) : (g |= 3 & t.button, 4 & t.button && (g |= 64), 8 & t.button && (g |= 128), t.action === 32 ? g |= 32 : t.action !== 0 || h || (g |= 3)), g;
                     }
                     const s = String.fromCharCode,
                         r = {
-                            DEFAULT: (e) => {
-                                const h = [l(e, !1) + 32, e.col + 32, e.row + 32];
+                            DEFAULT: (t) => {
+                                const h = [l(t, !1) + 32, t.col + 32, t.row + 32];
                                 return h[0] > 255 || h[1] > 255 || h[2] > 255 ? "" : `\x1B[M${s(h[0])}${s(h[1])}${s(h[2])}`;
                             },
-                            SGR: (e) => {
-                                const h = e.action === 0 && e.button !== 4 ? "m" : "M";
-                                return `\x1B[<${l(e, !0)};${e.col};${e.row}${h}`;
+                            SGR: (t) => {
+                                const h = t.action === 0 && t.button !== 4 ? "m" : "M";
+                                return `\x1B[<${l(t, !0)};${t.col};${t.row}${h}`;
                             },
-                            SGR_PIXELS: (e) => {
-                                const h = e.action === 0 && e.button !== 4 ? "m" : "M";
-                                return `\x1B[<${l(e, !0)};${e.x};${e.y}${h}`;
+                            SGR_PIXELS: (t) => {
+                                const h = t.action === 0 && t.button !== 4 ? "m" : "M";
+                                return `\x1B[<${l(t, !0)};${t.x};${t.y}${h}`;
                             }
                         };
-                    let t = i.CoreMouseService = class extends f.Disposable {
-                        constructor(e, h) {
-                            super(), this._bufferService = e, this._coreService = h, this._protocols = {}, this._encodings = {}, this._activeProtocol = "", this._activeEncoding = "", this._lastEvent = null, this._onProtocolChange = this.register(new d.EventEmitter()), this.onProtocolChange = this._onProtocolChange.event;
-                            for (const v of Object.keys(g))
-                                this.addProtocol(v, g[v]);
-                            for (const v of Object.keys(r))
-                                this.addEncoding(v, r[v]);
+                    let e = i.CoreMouseService = class extends v.Disposable {
+                        constructor(t, h) {
+                            super(), this._bufferService = t, this._coreService = h, this._protocols = {}, this._encodings = {}, this._activeProtocol = "", this._activeEncoding = "", this._lastEvent = null, this._onProtocolChange = this.register(new d.EventEmitter()), this.onProtocolChange = this._onProtocolChange.event;
+                            for (const g of Object.keys(m))
+                                this.addProtocol(g, m[g]);
+                            for (const g of Object.keys(r))
+                                this.addEncoding(g, r[g]);
                             this.reset();
                         }
-                        addProtocol(e, h) {
-                            this._protocols[e] = h;
+                        addProtocol(t, h) {
+                            this._protocols[t] = h;
                         }
-                        addEncoding(e, h) {
-                            this._encodings[e] = h;
+                        addEncoding(t, h) {
+                            this._encodings[t] = h;
                         }
                         get activeProtocol() {
                             return this._activeProtocol;
                         }
                         get areMouseEventsActive() {
                             return this._protocols[this._activeProtocol].events !== 0;
                         }
-                        set activeProtocol(e) {
-                            if (!this._protocols[e])
-                                throw new Error(`unknown protocol "${e}"`);
-                            this._activeProtocol = e, this._onProtocolChange.fire(this._protocols[e].events);
+                        set activeProtocol(t) {
+                            if (!this._protocols[t])
+                                throw new Error(`unknown protocol "${t}"`);
+                            this._activeProtocol = t, this._onProtocolChange.fire(this._protocols[t].events);
                         }
                         get activeEncoding() {
                             return this._activeEncoding;
                         }
-                        set activeEncoding(e) {
-                            if (!this._encodings[e])
-                                throw new Error(`unknown encoding "${e}"`);
-                            this._activeEncoding = e;
+                        set activeEncoding(t) {
+                            if (!this._encodings[t])
+                                throw new Error(`unknown encoding "${t}"`);
+                            this._activeEncoding = t;
                         }
                         reset() {
                             this.activeProtocol = "NONE", this.activeEncoding = "DEFAULT", this._lastEvent = null;
                         }
-                        triggerMouseEvent(e) {
-                            if (e.col < 0 || e.col >= this._bufferService.cols || e.row < 0 || e.row >= this._bufferService.rows || e.button === 4 && e.action === 32 || e.button === 3 && e.action !== 32 || e.button !== 4 && (e.action === 2 || e.action === 3) || (e.col++, e.row++, e.action === 32 && this._lastEvent && this._equalEvents(this._lastEvent, e, this._activeEncoding === "SGR_PIXELS")) || !this._protocols[this._activeProtocol].restrict(e))
+                        triggerMouseEvent(t) {
+                            if (t.col < 0 || t.col >= this._bufferService.cols || t.row < 0 || t.row >= this._bufferService.rows || t.button === 4 && t.action === 32 || t.button === 3 && t.action !== 32 || t.button !== 4 && (t.action === 2 || t.action === 3) || (t.col++, t.row++, t.action === 32 && this._lastEvent && this._equalEvents(this._lastEvent, t, this._activeEncoding === "SGR_PIXELS")) || !this._protocols[this._activeProtocol].restrict(t))
                                 return !1;
-                            const h = this._encodings[this._activeEncoding](e);
-                            return h && (this._activeEncoding === "DEFAULT" ? this._coreService.triggerBinaryEvent(h) : this._coreService.triggerDataEvent(h, !0)), this._lastEvent = e, !0;
+                            const h = this._encodings[this._activeEncoding](t);
+                            return h && (this._activeEncoding === "DEFAULT" ? this._coreService.triggerBinaryEvent(h) : this._coreService.triggerDataEvent(h, !0)), this._lastEvent = t, !0;
                         }
-                        explainEvents(e) {
+                        explainEvents(t) {
                             return {
-                                down: !!(1 & e),
-                                up: !!(2 & e),
-                                drag: !!(4 & e),
-                                move: !!(8 & e),
-                                wheel: !!(16 & e)
+                                down: !!(1 & t),
+                                up: !!(2 & t),
+                                drag: !!(4 & t),
+                                move: !!(8 & t),
+                                wheel: !!(16 & t)
                             };
                         }
-                        _equalEvents(e, h, v) {
-                            if (v) {
-                                if (e.x !== h.x || e.y !== h.y)
+                        _equalEvents(t, h, g) {
+                            if (g) {
+                                if (t.x !== h.x || t.y !== h.y)
                                     return !1;
-                            } else if (e.col !== h.col || e.row !== h.row)
+                            } else if (t.col !== h.col || t.row !== h.row)
                                 return !1;
-                            return e.button === h.button && e.action === h.action && e.ctrl === h.ctrl && e.alt === h.alt && e.shift === h.shift;
+                            return t.button === h.button && t.action === h.action && t.ctrl === h.ctrl && t.alt === h.alt && t.shift === h.shift;
                         }
                     };
-                    i.CoreMouseService = t = o([c(0, a.IBufferService), c(1, a.ICoreService)], t);
+                    i.CoreMouseService = e = o([c(0, a.IBufferService), c(1, a.ICoreService)], e);
                 },
                 6975: function(k, i, n) {
-                    var o = this && this.__decorate || function(t, e, h, v) {
-                            var u, p = arguments.length,
-                                _ = p < 3 ? e : v === null ? v = Object.getOwnPropertyDescriptor(e, h) : v;
+                    var o = this && this.__decorate || function(e, t, h, g) {
+                            var u, S = arguments.length,
+                                _ = S < 3 ? t : g === null ? g = Object.getOwnPropertyDescriptor(t, h) : g;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                _ = Reflect.decorate(t, e, h, v);
+                                _ = Reflect.decorate(e, t, h, g);
                             else
-                                for (var b = t.length - 1; b >= 0; b--)
-                                    (u = t[b]) && (_ = (p < 3 ? u(_) : p > 3 ? u(e, h, _) : u(e, h)) || _);
-                            return p > 3 && _ && Object.defineProperty(e, h, _), _;
+                                for (var b = e.length - 1; b >= 0; b--)
+                                    (u = e[b]) && (_ = (S < 3 ? u(_) : S > 3 ? u(t, h, _) : u(t, h)) || _);
+                            return S > 3 && _ && Object.defineProperty(t, h, _), _;
                         },
-                        c = this && this.__param || function(t, e) {
-                            return function(h, v) {
-                                e(h, v, t);
+                        c = this && this.__param || function(e, t) {
+                            return function(h, g) {
+                                t(h, g, e);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.CoreService = void 0;
                     const a = n(1439),
                         d = n(8460),
-                        f = n(844),
-                        g = n(2585),
+                        v = n(844),
+                        m = n(2585),
                         l = Object.freeze({
                             insertMode: !1
                         }),
                         s = Object.freeze({
                             applicationCursorKeys: !1,
                             applicationKeypad: !1,
                             bracketedPasteMode: !1,
                             origin: !1,
                             reverseWraparound: !1,
                             sendFocus: !1,
                             wraparound: !0
                         });
-                    let r = i.CoreService = class extends f.Disposable {
-                        constructor(t, e, h) {
-                            super(), this._bufferService = t, this._logService = e, this._optionsService = h, this.isCursorInitialized = !1, this.isCursorHidden = !1, this._onData = this.register(new d.EventEmitter()), this.onData = this._onData.event, this._onUserInput = this.register(new d.EventEmitter()), this.onUserInput = this._onUserInput.event, this._onBinary = this.register(new d.EventEmitter()), this.onBinary = this._onBinary.event, this._onRequestScrollToBottom = this.register(new d.EventEmitter()), this.onRequestScrollToBottom = this._onRequestScrollToBottom.event, this.modes = (0, a.clone)(l), this.decPrivateModes = (0, a.clone)(s);
+                    let r = i.CoreService = class extends v.Disposable {
+                        constructor(e, t, h) {
+                            super(), this._bufferService = e, this._logService = t, this._optionsService = h, this.isCursorInitialized = !1, this.isCursorHidden = !1, this._onData = this.register(new d.EventEmitter()), this.onData = this._onData.event, this._onUserInput = this.register(new d.EventEmitter()), this.onUserInput = this._onUserInput.event, this._onBinary = this.register(new d.EventEmitter()), this.onBinary = this._onBinary.event, this._onRequestScrollToBottom = this.register(new d.EventEmitter()), this.onRequestScrollToBottom = this._onRequestScrollToBottom.event, this.modes = (0, a.clone)(l), this.decPrivateModes = (0, a.clone)(s);
                         }
                         reset() {
                             this.modes = (0, a.clone)(l), this.decPrivateModes = (0, a.clone)(s);
                         }
-                        triggerDataEvent(t, e = !1) {
+                        triggerDataEvent(e, t = !1) {
                             if (this._optionsService.rawOptions.disableStdin)
                                 return;
                             const h = this._bufferService.buffer;
-                            e && this._optionsService.rawOptions.scrollOnUserInput && h.ybase !== h.ydisp && this._onRequestScrollToBottom.fire(), e && this._onUserInput.fire(), this._logService.debug(`sending data "${t}"`, () => t.split("").map((v) => v.charCodeAt(0))), this._onData.fire(t);
+                            t && this._optionsService.rawOptions.scrollOnUserInput && h.ybase !== h.ydisp && this._onRequestScrollToBottom.fire(), t && this._onUserInput.fire(), this._logService.debug(`sending data "${e}"`, () => e.split("").map((g) => g.charCodeAt(0))), this._onData.fire(e);
                         }
-                        triggerBinaryEvent(t) {
-                            this._optionsService.rawOptions.disableStdin || (this._logService.debug(`sending binary "${t}"`, () => t.split("").map((e) => e.charCodeAt(0))), this._onBinary.fire(t));
+                        triggerBinaryEvent(e) {
+                            this._optionsService.rawOptions.disableStdin || (this._logService.debug(`sending binary "${e}"`, () => e.split("").map((t) => t.charCodeAt(0))), this._onBinary.fire(e));
                         }
                     };
-                    i.CoreService = r = o([c(0, g.IBufferService), c(1, g.ILogService), c(2, g.IOptionsService)], r);
+                    i.CoreService = r = o([c(0, m.IBufferService), c(1, m.ILogService), c(2, m.IOptionsService)], r);
                 },
                 9074: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.DecorationService = void 0;
                     const o = n(8055),
                         c = n(8460),
                         a = n(844),
                         d = n(6106);
-                    let f = 0,
-                        g = 0;
+                    let v = 0,
+                        m = 0;
                     class l extends a.Disposable {
                         get decorations() {
                             return this._decorations.values();
                         }
                         constructor() {
-                            super(), this._decorations = new d.SortedList((t) => t == null ? void 0 : t.marker.line), this._onDecorationRegistered = this.register(new c.EventEmitter()), this.onDecorationRegistered = this._onDecorationRegistered.event, this._onDecorationRemoved = this.register(new c.EventEmitter()), this.onDecorationRemoved = this._onDecorationRemoved.event, this.register((0, a.toDisposable)(() => this.reset()));
+                            super(), this._decorations = new d.SortedList((e) => e == null ? void 0 : e.marker.line), this._onDecorationRegistered = this.register(new c.EventEmitter()), this.onDecorationRegistered = this._onDecorationRegistered.event, this._onDecorationRemoved = this.register(new c.EventEmitter()), this.onDecorationRemoved = this._onDecorationRemoved.event, this.register((0, a.toDisposable)(() => this.reset()));
                         }
-                        registerDecoration(t) {
-                            if (t.marker.isDisposed)
+                        registerDecoration(e) {
+                            if (e.marker.isDisposed)
                                 return;
-                            const e = new s(t);
-                            if (e) {
-                                const h = e.marker.onDispose(() => e.dispose());
-                                e.onDispose(() => {
-                                    e && (this._decorations.delete(e) && this._onDecorationRemoved.fire(e), h.dispose());
-                                }), this._decorations.insert(e), this._onDecorationRegistered.fire(e);
+                            const t = new s(e);
+                            if (t) {
+                                const h = t.marker.onDispose(() => t.dispose());
+                                t.onDispose(() => {
+                                    t && (this._decorations.delete(t) && this._onDecorationRemoved.fire(t), h.dispose());
+                                }), this._decorations.insert(t), this._onDecorationRegistered.fire(t);
                             }
-                            return e;
+                            return t;
                         }
                         reset() {
-                            for (const t of this._decorations.values())
-                                t.dispose();
+                            for (const e of this._decorations.values())
+                                e.dispose();
                             this._decorations.clear();
                         }
-                        * getDecorationsAtCell(t, e, h) {
-                            let v = 0,
+                        * getDecorationsAtCell(e, t, h) {
+                            let g = 0,
                                 u = 0;
-                            for (const p of this._decorations.getKeyIterator(e))
-                                v = p.options.x ?? 0, u = v + (p.options.width ?? 1), t >= v && t < u && (!h || (p.options.layer ?? "bottom") === h) && (yield p);
+                            for (const S of this._decorations.getKeyIterator(t))
+                                g = S.options.x ?? 0, u = g + (S.options.width ?? 1), e >= g && e < u && (!h || (S.options.layer ?? "bottom") === h) && (yield S);
                         }
-                        forEachDecorationAtCell(t, e, h, v) {
-                            this._decorations.forEachByKey(e, (u) => {
-                                f = u.options.x ?? 0, g = f + (u.options.width ?? 1), t >= f && t < g && (!h || (u.options.layer ?? "bottom") === h) && v(u);
+                        forEachDecorationAtCell(e, t, h, g) {
+                            this._decorations.forEachByKey(t, (u) => {
+                                v = u.options.x ?? 0, m = v + (u.options.width ?? 1), e >= v && e < m && (!h || (u.options.layer ?? "bottom") === h) && g(u);
                             });
                         }
                     }
                     i.DecorationService = l;
                     class s extends a.Disposable {
                         get isDisposed() {
                             return this._isDisposed;
                         }
                         get backgroundColorRGB() {
                             return this._cachedBg === null && (this.options.backgroundColor ? this._cachedBg = o.css.toColor(this.options.backgroundColor) : this._cachedBg = void 0), this._cachedBg;
                         }
                         get foregroundColorRGB() {
                             return this._cachedFg === null && (this.options.foregroundColor ? this._cachedFg = o.css.toColor(this.options.foregroundColor) : this._cachedFg = void 0), this._cachedFg;
                         }
-                        constructor(t) {
-                            super(), this.options = t, this.onRenderEmitter = this.register(new c.EventEmitter()), this.onRender = this.onRenderEmitter.event, this._onDispose = this.register(new c.EventEmitter()), this.onDispose = this._onDispose.event, this._cachedBg = null, this._cachedFg = null, this.marker = t.marker, this.options.overviewRulerOptions && !this.options.overviewRulerOptions.position && (this.options.overviewRulerOptions.position = "full");
+                        constructor(e) {
+                            super(), this.options = e, this.onRenderEmitter = this.register(new c.EventEmitter()), this.onRender = this.onRenderEmitter.event, this._onDispose = this.register(new c.EventEmitter()), this.onDispose = this._onDispose.event, this._cachedBg = null, this._cachedFg = null, this.marker = e.marker, this.options.overviewRulerOptions && !this.options.overviewRulerOptions.position && (this.options.overviewRulerOptions.position = "full");
                         }
                         dispose() {
                             this._onDispose.fire(), super.dispose();
                         }
                     }
                 },
                 4348: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.InstantiationService = i.ServiceCollection = void 0;
                     const o = n(2585),
                         c = n(8343);
                     class a {
-                        constructor(...f) {
+                        constructor(...v) {
                             this._entries = /* @__PURE__ */ new Map();
-                            for (const [g, l] of f)
-                                this.set(g, l);
+                            for (const [m, l] of v)
+                                this.set(m, l);
                         }
-                        set(f, g) {
-                            const l = this._entries.get(f);
-                            return this._entries.set(f, g), l;
-                        }
-                        forEach(f) {
-                            for (const [g, l] of this._entries.entries())
-                                f(g, l);
+                        set(v, m) {
+                            const l = this._entries.get(v);
+                            return this._entries.set(v, m), l;
+                        }
+                        forEach(v) {
+                            for (const [m, l] of this._entries.entries())
+                                v(m, l);
                         }
-                        has(f) {
-                            return this._entries.has(f);
+                        has(v) {
+                            return this._entries.has(v);
                         }
-                        get(f) {
-                            return this._entries.get(f);
+                        get(v) {
+                            return this._entries.get(v);
                         }
                     }
                     i.ServiceCollection = a, i.InstantiationService = class {
                         constructor() {
                             this._services = new a(), this._services.set(o.IInstantiationService, this);
                         }
-                        setService(d, f) {
-                            this._services.set(d, f);
+                        setService(d, v) {
+                            this._services.set(d, v);
                         }
                         getService(d) {
                             return this._services.get(d);
                         }
-                        createInstance(d, ...f) {
-                            const g = (0, c.getServiceDependencies)(d).sort((r, t) => r.index - t.index),
+                        createInstance(d, ...v) {
+                            const m = (0, c.getServiceDependencies)(d).sort((r, e) => r.index - e.index),
                                 l = [];
-                            for (const r of g) {
-                                const t = this._services.get(r.id);
-                                if (!t)
+                            for (const r of m) {
+                                const e = this._services.get(r.id);
+                                if (!e)
                                     throw new Error(`[createInstance] ${d.name} depends on UNKNOWN service ${r.id}.`);
-                                l.push(t);
+                                l.push(e);
                             }
-                            const s = g.length > 0 ? g[0].index : f.length;
-                            if (f.length !== s)
-                                throw new Error(`[createInstance] First service dependency of ${d.name} at position ${s + 1} conflicts with ${f.length} static arguments`);
-                            return new d(...f, ...l);
+                            const s = m.length > 0 ? m[0].index : v.length;
+                            if (v.length !== s)
+                                throw new Error(`[createInstance] First service dependency of ${d.name} at position ${s + 1} conflicts with ${v.length} static arguments`);
+                            return new d(...v, ...l);
                         }
                     };
                 },
                 7866: function(k, i, n) {
-                    var o = this && this.__decorate || function(s, r, t, e) {
-                            var h, v = arguments.length,
-                                u = v < 3 ? r : e === null ? e = Object.getOwnPropertyDescriptor(r, t) : e;
+                    var o = this && this.__decorate || function(s, r, e, t) {
+                            var h, g = arguments.length,
+                                u = g < 3 ? r : t === null ? t = Object.getOwnPropertyDescriptor(r, e) : t;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                u = Reflect.decorate(s, r, t, e);
+                                u = Reflect.decorate(s, r, e, t);
                             else
-                                for (var p = s.length - 1; p >= 0; p--)
-                                    (h = s[p]) && (u = (v < 3 ? h(u) : v > 3 ? h(r, t, u) : h(r, t)) || u);
-                            return v > 3 && u && Object.defineProperty(r, t, u), u;
+                                for (var S = s.length - 1; S >= 0; S--)
+                                    (h = s[S]) && (u = (g < 3 ? h(u) : g > 3 ? h(r, e, u) : h(r, e)) || u);
+                            return g > 3 && u && Object.defineProperty(r, e, u), u;
                         },
                         c = this && this.__param || function(s, r) {
-                            return function(t, e) {
-                                r(t, e, s);
+                            return function(e, t) {
+                                r(e, t, s);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.traceCall = i.setTraceLogger = i.LogService = void 0;
                     const a = n(844),
                         d = n(2585),
-                        f = {
+                        v = {
                             trace: d.LogLevelEnum.TRACE,
                             debug: d.LogLevelEnum.DEBUG,
                             info: d.LogLevelEnum.INFO,
                             warn: d.LogLevelEnum.WARN,
                             error: d.LogLevelEnum.ERROR,
                             off: d.LogLevelEnum.OFF
                         };
-                    let g, l = i.LogService = class extends a.Disposable {
+                    let m, l = i.LogService = class extends a.Disposable {
                         get logLevel() {
                             return this._logLevel;
                         }
                         constructor(s) {
-                            super(), this._optionsService = s, this._logLevel = d.LogLevelEnum.OFF, this._updateLogLevel(), this.register(this._optionsService.onSpecificOptionChange("logLevel", () => this._updateLogLevel())), g = this;
+                            super(), this._optionsService = s, this._logLevel = d.LogLevelEnum.OFF, this._updateLogLevel(), this.register(this._optionsService.onSpecificOptionChange("logLevel", () => this._updateLogLevel())), m = this;
                         }
                         _updateLogLevel() {
-                            this._logLevel = f[this._optionsService.rawOptions.logLevel];
+                            this._logLevel = v[this._optionsService.rawOptions.logLevel];
                         }
                         _evalLazyOptionalParams(s) {
                             for (let r = 0; r < s.length; r++)
                                 typeof s[r] == "function" && (s[r] = s[r]());
                         }
-                        _log(s, r, t) {
-                            this._evalLazyOptionalParams(t), s.call(console, (this._optionsService.options.logger ? "" : "xterm.js: ") + r, ...t);
+                        _log(s, r, e) {
+                            this._evalLazyOptionalParams(e), s.call(console, (this._optionsService.options.logger ? "" : "xterm.js: ") + r, ...e);
                         }
                         trace(s, ...r) {
-                            var t;
-                            this._logLevel <= d.LogLevelEnum.TRACE && this._log(((t = this._optionsService.options.logger) == null ? void 0 : t.trace.bind(this._optionsService.options.logger)) ?? console.log, s, r);
+                            var e;
+                            this._logLevel <= d.LogLevelEnum.TRACE && this._log(((e = this._optionsService.options.logger) == null ? void 0 : e.trace.bind(this._optionsService.options.logger)) ?? console.log, s, r);
                         }
                         debug(s, ...r) {
-                            var t;
-                            this._logLevel <= d.LogLevelEnum.DEBUG && this._log(((t = this._optionsService.options.logger) == null ? void 0 : t.debug.bind(this._optionsService.options.logger)) ?? console.log, s, r);
+                            var e;
+                            this._logLevel <= d.LogLevelEnum.DEBUG && this._log(((e = this._optionsService.options.logger) == null ? void 0 : e.debug.bind(this._optionsService.options.logger)) ?? console.log, s, r);
                         }
                         info(s, ...r) {
-                            var t;
-                            this._logLevel <= d.LogLevelEnum.INFO && this._log(((t = this._optionsService.options.logger) == null ? void 0 : t.info.bind(this._optionsService.options.logger)) ?? console.info, s, r);
+                            var e;
+                            this._logLevel <= d.LogLevelEnum.INFO && this._log(((e = this._optionsService.options.logger) == null ? void 0 : e.info.bind(this._optionsService.options.logger)) ?? console.info, s, r);
                         }
                         warn(s, ...r) {
-                            var t;
-                            this._logLevel <= d.LogLevelEnum.WARN && this._log(((t = this._optionsService.options.logger) == null ? void 0 : t.warn.bind(this._optionsService.options.logger)) ?? console.warn, s, r);
+                            var e;
+                            this._logLevel <= d.LogLevelEnum.WARN && this._log(((e = this._optionsService.options.logger) == null ? void 0 : e.warn.bind(this._optionsService.options.logger)) ?? console.warn, s, r);
                         }
                         error(s, ...r) {
-                            var t;
-                            this._logLevel <= d.LogLevelEnum.ERROR && this._log(((t = this._optionsService.options.logger) == null ? void 0 : t.error.bind(this._optionsService.options.logger)) ?? console.error, s, r);
+                            var e;
+                            this._logLevel <= d.LogLevelEnum.ERROR && this._log(((e = this._optionsService.options.logger) == null ? void 0 : e.error.bind(this._optionsService.options.logger)) ?? console.error, s, r);
                         }
                     };
                     i.LogService = l = o([c(0, d.IOptionsService)], l), i.setTraceLogger = function(s) {
-                        g = s;
-                    }, i.traceCall = function(s, r, t) {
-                        if (typeof t.value != "function")
+                        m = s;
+                    }, i.traceCall = function(s, r, e) {
+                        if (typeof e.value != "function")
                             throw new Error("not supported");
-                        const e = t.value;
-                        t.value = function(...h) {
-                            if (g.logLevel !== d.LogLevelEnum.TRACE)
-                                return e.apply(this, h);
-                            g.trace(`GlyphRenderer#${e.name}(${h.map((u) => JSON.stringify(u)).join(", ")})`);
-                            const v = e.apply(this, h);
-                            return g.trace(`GlyphRenderer#${e.name} return`, v), v;
+                        const t = e.value;
+                        e.value = function(...h) {
+                            if (m.logLevel !== d.LogLevelEnum.TRACE)
+                                return t.apply(this, h);
+                            m.trace(`GlyphRenderer#${t.name}(${h.map((u) => JSON.stringify(u)).join(", ")})`);
+                            const g = t.apply(this, h);
+                            return m.trace(`GlyphRenderer#${t.name} return`, g), g;
                         };
                     };
                 },
                 7302: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.OptionsService = i.DEFAULT_OPTIONS = void 0;
@@ -10212,27 +10212,27 @@
                         altClickMovesCursor: !0,
                         convertEol: !1,
                         termName: "xterm",
                         cancelEvents: !1,
                         overviewRulerWidth: 0
                     };
                     const d = ["normal", "bold", "100", "200", "300", "400", "500", "600", "700", "800", "900"];
-                    class f extends c.Disposable {
+                    class v extends c.Disposable {
                         constructor(l) {
                             super(), this._onOptionChange = this.register(new o.EventEmitter()), this.onOptionChange = this._onOptionChange.event;
                             const s = {
                                 ...i.DEFAULT_OPTIONS
                             };
                             for (const r in l)
                                 if (r in s)
                                     try {
-                                        const t = l[r];
-                                        s[r] = this._sanitizeAndValidateOption(r, t);
-                                    } catch (t) {
-                                        console.error(t);
+                                        const e = l[r];
+                                        s[r] = this._sanitizeAndValidateOption(r, e);
+                                    } catch (e) {
+                                        console.error(e);
                                     }
                             this.rawOptions = s, this.options = {
                                 ...s
                             }, this._setupOptions(), this.register((0, c.toDisposable)(() => {
                                 this.rawOptions.linkHandler = null, this.rawOptions.documentOverride = null;
                             }));
                         }
@@ -10248,25 +10248,25 @@
                         }
                         _setupOptions() {
                             const l = (r) => {
                                     if (!(r in i.DEFAULT_OPTIONS))
                                         throw new Error(`No option with key "${r}"`);
                                     return this.rawOptions[r];
                                 },
-                                s = (r, t) => {
+                                s = (r, e) => {
                                     if (!(r in i.DEFAULT_OPTIONS))
                                         throw new Error(`No option with key "${r}"`);
-                                    t = this._sanitizeAndValidateOption(r, t), this.rawOptions[r] !== t && (this.rawOptions[r] = t, this._onOptionChange.fire(r));
+                                    e = this._sanitizeAndValidateOption(r, e), this.rawOptions[r] !== e && (this.rawOptions[r] = e, this._onOptionChange.fire(r));
                                 };
                             for (const r in this.rawOptions) {
-                                const t = {
+                                const e = {
                                     get: l.bind(this, r),
                                     set: s.bind(this, r)
                                 };
-                                Object.defineProperty(this.options, r, t);
+                                Object.defineProperty(this.options, r, e);
                             }
                         }
                         _sanitizeAndValidateOption(l, s) {
                             switch (l) {
                                 case "cursorStyle":
                                     if (s || (s = i.DEFAULT_OPTIONS[l]), ! /* @__PURE__ */ function(r) {
                                             return r === "block" || r === "underline" || r === "bar";
@@ -10308,82 +10308,82 @@
                                     break;
                                 case "windowsPty":
                                     s = s ?? {};
                             }
                             return s;
                         }
                     }
-                    i.OptionsService = f;
+                    i.OptionsService = v;
                 },
                 2660: function(k, i, n) {
-                    var o = this && this.__decorate || function(f, g, l, s) {
-                            var r, t = arguments.length,
-                                e = t < 3 ? g : s === null ? s = Object.getOwnPropertyDescriptor(g, l) : s;
+                    var o = this && this.__decorate || function(v, m, l, s) {
+                            var r, e = arguments.length,
+                                t = e < 3 ? m : s === null ? s = Object.getOwnPropertyDescriptor(m, l) : s;
                             if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-                                e = Reflect.decorate(f, g, l, s);
+                                t = Reflect.decorate(v, m, l, s);
                             else
-                                for (var h = f.length - 1; h >= 0; h--)
-                                    (r = f[h]) && (e = (t < 3 ? r(e) : t > 3 ? r(g, l, e) : r(g, l)) || e);
-                            return t > 3 && e && Object.defineProperty(g, l, e), e;
+                                for (var h = v.length - 1; h >= 0; h--)
+                                    (r = v[h]) && (t = (e < 3 ? r(t) : e > 3 ? r(m, l, t) : r(m, l)) || t);
+                            return e > 3 && t && Object.defineProperty(m, l, t), t;
                         },
-                        c = this && this.__param || function(f, g) {
+                        c = this && this.__param || function(v, m) {
                             return function(l, s) {
-                                g(l, s, f);
+                                m(l, s, v);
                             };
                         };
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.OscLinkService = void 0;
                     const a = n(2585);
                     let d = i.OscLinkService = class {
-                        constructor(f) {
-                            this._bufferService = f, this._nextId = 1, this._entriesWithId = /* @__PURE__ */ new Map(), this._dataByLinkId = /* @__PURE__ */ new Map();
+                        constructor(v) {
+                            this._bufferService = v, this._nextId = 1, this._entriesWithId = /* @__PURE__ */ new Map(), this._dataByLinkId = /* @__PURE__ */ new Map();
                         }
-                        registerLink(f) {
-                            const g = this._bufferService.buffer;
-                            if (f.id === void 0) {
-                                const h = g.addMarker(g.ybase + g.y),
-                                    v = {
-                                        data: f,
+                        registerLink(v) {
+                            const m = this._bufferService.buffer;
+                            if (v.id === void 0) {
+                                const h = m.addMarker(m.ybase + m.y),
+                                    g = {
+                                        data: v,
                                         id: this._nextId++,
                                         lines: [h]
                                     };
-                                return h.onDispose(() => this._removeMarkerFromLink(v, h)), this._dataByLinkId.set(v.id, v), v.id;
+                                return h.onDispose(() => this._removeMarkerFromLink(g, h)), this._dataByLinkId.set(g.id, g), g.id;
                             }
-                            const l = f,
+                            const l = v,
                                 s = this._getEntryIdKey(l),
                                 r = this._entriesWithId.get(s);
                             if (r)
-                                return this.addLineToLink(r.id, g.ybase + g.y), r.id;
-                            const t = g.addMarker(g.ybase + g.y),
-                                e = {
+                                return this.addLineToLink(r.id, m.ybase + m.y), r.id;
+                            const e = m.addMarker(m.ybase + m.y),
+                                t = {
                                     id: this._nextId++,
                                     key: this._getEntryIdKey(l),
                                     data: l,
-                                    lines: [t]
+                                    lines: [e]
                                 };
-                            return t.onDispose(() => this._removeMarkerFromLink(e, t)), this._entriesWithId.set(e.key, e), this._dataByLinkId.set(e.id, e), e.id;
+                            return e.onDispose(() => this._removeMarkerFromLink(t, e)), this._entriesWithId.set(t.key, t), this._dataByLinkId.set(t.id, t), t.id;
                         }
-                        addLineToLink(f, g) {
-                            const l = this._dataByLinkId.get(f);
-                            if (l && l.lines.every((s) => s.line !== g)) {
-                                const s = this._bufferService.buffer.addMarker(g);
+                        addLineToLink(v, m) {
+                            const l = this._dataByLinkId.get(v);
+                            if (l && l.lines.every((s) => s.line !== m)) {
+                                const s = this._bufferService.buffer.addMarker(m);
                                 l.lines.push(s), s.onDispose(() => this._removeMarkerFromLink(l, s));
                             }
                         }
-                        getLinkData(f) {
-                            var g;
-                            return (g = this._dataByLinkId.get(f)) == null ? void 0 : g.data;
-                        }
-                        _getEntryIdKey(f) {
-                            return `${f.id};;${f.uri}`;
-                        }
-                        _removeMarkerFromLink(f, g) {
-                            const l = f.lines.indexOf(g);
-                            l !== -1 && (f.lines.splice(l, 1), f.lines.length === 0 && (f.data.id !== void 0 && this._entriesWithId.delete(f.key), this._dataByLinkId.delete(f.id)));
+                        getLinkData(v) {
+                            var m;
+                            return (m = this._dataByLinkId.get(v)) == null ? void 0 : m.data;
+                        }
+                        _getEntryIdKey(v) {
+                            return `${v.id};;${v.uri}`;
+                        }
+                        _removeMarkerFromLink(v, m) {
+                            const l = v.lines.indexOf(m);
+                            l !== -1 && (v.lines.splice(l, 1), v.lines.length === 0 && (v.data.id !== void 0 && this._entriesWithId.delete(v.key), this._dataByLinkId.delete(v.id)));
                         }
                     };
                     i.OscLinkService = d = o([c(0, a.IBufferService)], d);
                 },
                 8343: (k, i) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
@@ -10391,26 +10391,26 @@
                     const n = "di$target",
                         o = "di$dependencies";
                     i.serviceRegistry = /* @__PURE__ */ new Map(), i.getServiceDependencies = function(c) {
                         return c[o] || [];
                     }, i.createDecorator = function(c) {
                         if (i.serviceRegistry.has(c))
                             return i.serviceRegistry.get(c);
-                        const a = function(d, f, g) {
+                        const a = function(d, v, m) {
                             if (arguments.length !== 3)
                                 throw new Error("@IServiceName-decorator can only be used to decorate a parameter");
                             (function(l, s, r) {
                                 s[n] === s ? s[o].push({
                                     id: l,
                                     index: r
                                 }) : (s[o] = [{
                                     id: l,
                                     index: r
                                 }], s[n] = s);
-                            })(a, d, g);
+                            })(a, d, m);
                         };
                         return a.toString = () => c, i.serviceRegistry.set(c, a), a;
                     };
                 },
                 2585: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
@@ -10425,120 +10425,120 @@
                 1480: (k, i, n) => {
                     Object.defineProperty(i, "__esModule", {
                         value: !0
                     }), i.UnicodeService = void 0;
                     const o = n(8460),
                         c = n(225);
                     class a {
-                        static extractShouldJoin(f) {
-                            return (1 & f) != 0;
+                        static extractShouldJoin(v) {
+                            return (1 & v) != 0;
                         }
-                        static extractWidth(f) {
-                            return f >> 1 & 3;
+                        static extractWidth(v) {
+                            return v >> 1 & 3;
                         }
-                        static extractCharKind(f) {
-                            return f >> 3;
+                        static extractCharKind(v) {
+                            return v >> 3;
                         }
-                        static createPropertyValue(f, g, l = !1) {
-                            return (16777215 & f) << 3 | (3 & g) << 1 | (l ? 1 : 0);
+                        static createPropertyValue(v, m, l = !1) {
+                            return (16777215 & v) << 3 | (3 & m) << 1 | (l ? 1 : 0);
                         }
                         constructor() {
                             this._providers = /* @__PURE__ */ Object.create(null), this._active = "", this._onChange = new o.EventEmitter(), this.onChange = this._onChange.event;
-                            const f = new c.UnicodeV6();
-                            this.register(f), this._active = f.version, this._activeProvider = f;
+                            const v = new c.UnicodeV6();
+                            this.register(v), this._active = v.version, this._activeProvider = v;
                         }
                         dispose() {
                             this._onChange.dispose();
                         }
                         get versions() {
                             return Object.keys(this._providers);
                         }
                         get activeVersion() {
                             return this._active;
                         }
-                        set activeVersion(f) {
-                            if (!this._providers[f])
-                                throw new Error(`unknown Unicode version "${f}"`);
-                            this._active = f, this._activeProvider = this._providers[f], this._onChange.fire(f);
+                        set activeVersion(v) {
+                            if (!this._providers[v])
+                                throw new Error(`unknown Unicode version "${v}"`);
+                            this._active = v, this._activeProvider = this._providers[v], this._onChange.fire(v);
                         }
-                        register(f) {
-                            this._providers[f.version] = f;
+                        register(v) {
+                            this._providers[v.version] = v;
                         }
-                        wcwidth(f) {
-                            return this._activeProvider.wcwidth(f);
+                        wcwidth(v) {
+                            return this._activeProvider.wcwidth(v);
                         }
-                        getStringCellWidth(f) {
-                            let g = 0,
+                        getStringCellWidth(v) {
+                            let m = 0,
                                 l = 0;
-                            const s = f.length;
+                            const s = v.length;
                             for (let r = 0; r < s; ++r) {
-                                let t = f.charCodeAt(r);
-                                if (55296 <= t && t <= 56319) {
+                                let e = v.charCodeAt(r);
+                                if (55296 <= e && e <= 56319) {
                                     if (++r >= s)
-                                        return g + this.wcwidth(t);
-                                    const v = f.charCodeAt(r);
-                                    56320 <= v && v <= 57343 ? t = 1024 * (t - 55296) + v - 56320 + 65536 : g += this.wcwidth(v);
-                                }
-                                const e = this.charProperties(t, l);
-                                let h = a.extractWidth(e);
-                                a.extractShouldJoin(e) && (h -= a.extractWidth(l)), g += h, l = e;
+                                        return m + this.wcwidth(e);
+                                    const g = v.charCodeAt(r);
+                                    56320 <= g && g <= 57343 ? e = 1024 * (e - 55296) + g - 56320 + 65536 : m += this.wcwidth(g);
+                                }
+                                const t = this.charProperties(e, l);
+                                let h = a.extractWidth(t);
+                                a.extractShouldJoin(t) && (h -= a.extractWidth(l)), m += h, l = t;
                             }
-                            return g;
+                            return m;
                         }
-                        charProperties(f, g) {
-                            return this._activeProvider.charProperties(f, g);
+                        charProperties(v, m) {
+                            return this._activeProvider.charProperties(v, m);
                         }
                     }
                     i.UnicodeService = a;
                 }
             },
             y = {};
 
-        function R(k) {
+        function D(k) {
             var i = y[k];
             if (i !== void 0)
                 return i.exports;
             var n = y[k] = {
                 exports: {}
             };
-            return S[k].call(n.exports, n, n.exports, R), n.exports;
+            return p[k].call(n.exports, n, n.exports, D), n.exports;
         }
         var M = {};
         return (() => {
             var k = M;
             Object.defineProperty(k, "__esModule", {
                 value: !0
             }), k.Terminal = void 0;
-            const i = R(9042),
-                n = R(3236),
-                o = R(844),
-                c = R(5741),
-                a = R(8285),
-                d = R(7975),
-                f = R(7090),
-                g = ["cols", "rows"];
+            const i = D(9042),
+                n = D(3236),
+                o = D(844),
+                c = D(5741),
+                a = D(8285),
+                d = D(7975),
+                v = D(7090),
+                m = ["cols", "rows"];
             class l extends o.Disposable {
                 constructor(r) {
                     super(), this._core = this.register(new n.Terminal(r)), this._addonManager = this.register(new c.AddonManager()), this._publicOptions = {
                         ...this._core.options
                     };
-                    const t = (h) => this._core.options[h],
-                        e = (h, v) => {
-                            this._checkReadonlyOptions(h), this._core.options[h] = v;
+                    const e = (h) => this._core.options[h],
+                        t = (h, g) => {
+                            this._checkReadonlyOptions(h), this._core.options[h] = g;
                         };
                     for (const h in this._core.options) {
-                        const v = {
-                            get: t.bind(this, h),
-                            set: e.bind(this, h)
+                        const g = {
+                            get: e.bind(this, h),
+                            set: t.bind(this, h)
                         };
-                        Object.defineProperty(this._publicOptions, h, v);
+                        Object.defineProperty(this._publicOptions, h, g);
                     }
                 }
                 _checkReadonlyOptions(r) {
-                    if (g.includes(r))
+                    if (m.includes(r))
                         throw new Error(`Option "${r}" can only be set in the constructor`);
                 }
                 _checkProposedApi() {
                     if (!this._core.optionsService.rawOptions.allowProposedApi)
                         throw new Error("You must set the allowProposedApi option to true to use proposed API");
                 }
                 get onBell() {
@@ -10580,15 +10580,15 @@
                 get element() {
                     return this._core.element;
                 }
                 get parser() {
                     return this._parser || (this._parser = new d.ParserApi(this._core)), this._parser;
                 }
                 get unicode() {
-                    return this._checkProposedApi(), new f.UnicodeApi(this._core);
+                    return this._checkProposedApi(), new v.UnicodeApi(this._core);
                 }
                 get textarea() {
                     return this._core.textarea;
                 }
                 get rows() {
                     return this._core.rows;
                 }
@@ -10599,58 +10599,58 @@
                     return this._buffer || (this._buffer = this.register(new a.BufferNamespaceApi(this._core))), this._buffer;
                 }
                 get markers() {
                     return this._checkProposedApi(), this._core.markers;
                 }
                 get modes() {
                     const r = this._core.coreService.decPrivateModes;
-                    let t = "none";
+                    let e = "none";
                     switch (this._core.coreMouseService.activeProtocol) {
                         case "X10":
-                            t = "x10";
+                            e = "x10";
                             break;
                         case "VT200":
-                            t = "vt200";
+                            e = "vt200";
                             break;
                         case "DRAG":
-                            t = "drag";
+                            e = "drag";
                             break;
                         case "ANY":
-                            t = "any";
+                            e = "any";
                     }
                     return {
                         applicationCursorKeysMode: r.applicationCursorKeys,
                         applicationKeypadMode: r.applicationKeypad,
                         bracketedPasteMode: r.bracketedPasteMode,
                         insertMode: this._core.coreService.modes.insertMode,
-                        mouseTrackingMode: t,
+                        mouseTrackingMode: e,
                         originMode: r.origin,
                         reverseWraparoundMode: r.reverseWraparound,
                         sendFocusMode: r.sendFocus,
                         wraparoundMode: r.wraparound
                     };
                 }
                 get options() {
                     return this._publicOptions;
                 }
                 set options(r) {
-                    for (const t in r)
-                        this._publicOptions[t] = r[t];
+                    for (const e in r)
+                        this._publicOptions[e] = r[e];
                 }
                 blur() {
                     this._core.blur();
                 }
                 focus() {
                     this._core.focus();
                 }
-                input(r, t = !0) {
-                    this._core.input(r, t);
+                input(r, e = !0) {
+                    this._core.input(r, e);
                 }
-                resize(r, t) {
-                    this._verifyIntegers(r, t), this._core.resize(r, t);
+                resize(r, e) {
+                    this._verifyIntegers(r, e), this._core.resize(r, e);
                 }
                 open(r) {
                     this._core.open(r);
                 }
                 attachCustomKeyEventHandler(r) {
                     this._core.attachCustomKeyEventHandler(r);
                 }
@@ -10671,31 +10671,31 @@
                 }
                 registerDecoration(r) {
                     return this._checkProposedApi(), this._verifyPositiveIntegers(r.x ?? 0, r.width ?? 0, r.height ?? 0), this._core.registerDecoration(r);
                 }
                 hasSelection() {
                     return this._core.hasSelection();
                 }
-                select(r, t, e) {
-                    this._verifyIntegers(r, t, e), this._core.select(r, t, e);
+                select(r, e, t) {
+                    this._verifyIntegers(r, e, t), this._core.select(r, e, t);
                 }
                 getSelection() {
                     return this._core.getSelection();
                 }
                 getSelectionPosition() {
                     return this._core.getSelectionPosition();
                 }
                 clearSelection() {
                     this._core.clearSelection();
                 }
                 selectAll() {
                     this._core.selectAll();
                 }
-                selectLines(r, t) {
-                    this._verifyIntegers(r, t), this._core.selectLines(r, t);
+                selectLines(r, e) {
+                    this._verifyIntegers(r, e), this._core.selectLines(r, e);
                 }
                 dispose() {
                     super.dispose();
                 }
                 scrollLines(r) {
                     this._verifyIntegers(r), this._core.scrollLines(r);
                 }
@@ -10710,228 +10710,228 @@
                 }
                 scrollToLine(r) {
                     this._verifyIntegers(r), this._core.scrollToLine(r);
                 }
                 clear() {
                     this._core.clear();
                 }
-                write(r, t) {
-                    this._core.write(r, t);
+                write(r, e) {
+                    this._core.write(r, e);
                 }
-                writeln(r, t) {
+                writeln(r, e) {
                     this._core.write(r), this._core.write(`\r
-`, t);
+`, e);
                 }
                 paste(r) {
                     this._core.paste(r);
                 }
-                refresh(r, t) {
-                    this._verifyIntegers(r, t), this._core.refresh(r, t);
+                refresh(r, e) {
+                    this._verifyIntegers(r, e), this._core.refresh(r, e);
                 }
                 reset() {
                     this._core.reset();
                 }
                 clearTextureAtlas() {
                     this._core.clearTextureAtlas();
                 }
                 loadAddon(r) {
                     this._addonManager.loadAddon(this, r);
                 }
                 static get strings() {
                     return i;
                 }
                 _verifyIntegers(...r) {
-                    for (const t of r)
-                        if (t === 1 / 0 || isNaN(t) || t % 1 != 0)
+                    for (const e of r)
+                        if (e === 1 / 0 || isNaN(e) || e % 1 != 0)
                             throw new Error("This API only accepts integers");
                 }
                 _verifyPositiveIntegers(...r) {
-                    for (const t of r)
-                        if (t && (t === 1 / 0 || isNaN(t) || t % 1 != 0 || t < 0))
+                    for (const e of r)
+                        if (e && (e === 1 / 0 || isNaN(e) || e % 1 != 0 || e < 0))
                             throw new Error("This API only accepts positive integers");
                 }
             }
             k.Terminal = l;
         })(), M;
     })());
 })(Ut);
-var Ts = Ut.exports;
-const Ms = /* @__PURE__ */ Nt(Ts);
+var Bs = Ut.exports;
+const Ms = /* @__PURE__ */ Nt(Bs);
 var zt = {
     exports: {}
 };
-(function(E, m) {
-    (function(S, y) {
+(function(E, f) {
+    (function(p, y) {
         E.exports = y();
     })(self, () => (() => {
-        var S = {};
+        var p = {};
         return (() => {
-            var y = S;
+            var y = p;
             Object.defineProperty(y, "__esModule", {
                 value: !0
             }), y.FitAddon = void 0, y.FitAddon = class {
-                activate(R) {
-                    this._terminal = R;
+                activate(D) {
+                    this._terminal = D;
                 }
                 dispose() {}
                 fit() {
-                    const R = this.proposeDimensions();
-                    if (!R || !this._terminal || isNaN(R.cols) || isNaN(R.rows))
+                    const D = this.proposeDimensions();
+                    if (!D || !this._terminal || isNaN(D.cols) || isNaN(D.rows))
                         return;
                     const M = this._terminal._core;
-                    this._terminal.rows === R.rows && this._terminal.cols === R.cols || (M._renderService.clear(), this._terminal.resize(R.cols, R.rows));
+                    this._terminal.rows === D.rows && this._terminal.cols === D.cols || (M._renderService.clear(), this._terminal.resize(D.cols, D.rows));
                 }
                 proposeDimensions() {
                     if (!this._terminal || !this._terminal.element || !this._terminal.element.parentElement)
                         return;
-                    const R = this._terminal._core,
-                        M = R._renderService.dimensions;
+                    const D = this._terminal._core,
+                        M = D._renderService.dimensions;
                     if (M.css.cell.width === 0 || M.css.cell.height === 0)
                         return;
-                    const k = this._terminal.options.scrollback === 0 ? 0 : R.viewport.scrollBarWidth,
+                    const k = this._terminal.options.scrollback === 0 ? 0 : D.viewport.scrollBarWidth,
                         i = window.getComputedStyle(this._terminal.element.parentElement),
                         n = parseInt(i.getPropertyValue("height")),
                         o = Math.max(0, parseInt(i.getPropertyValue("width"))),
                         c = window.getComputedStyle(this._terminal.element),
                         a = n - (parseInt(c.getPropertyValue("padding-top")) + parseInt(c.getPropertyValue("padding-bottom"))),
                         d = o - (parseInt(c.getPropertyValue("padding-right")) + parseInt(c.getPropertyValue("padding-left"))) - k;
                     return {
                         cols: Math.max(2, Math.floor(d / M.css.cell.width)),
                         rows: Math.max(1, Math.floor(a / M.css.cell.height))
                     };
                 }
             };
-        })(), S;
+        })(), p;
     })());
 })(zt);
-var xs = zt.exports;
-const Os = /* @__PURE__ */ Nt(xs);
+var Ts = zt.exports;
+const Os = /* @__PURE__ */ Nt(Ts);
 const {
     SvelteComponent: Ps,
-    append: Dt,
+    append: xt,
     assign: Is,
-    attr: Rt,
+    attr: Dt,
     binding_callbacks: Hs,
     check_outros: Fs,
-    create_component: Qe,
+    create_component: $e,
     destroy_component: et,
-    detach: Ye,
-    element: At,
-    flush: ae,
+    detach: Ze,
+    element: Rt,
+    flush: Y,
     get_spread_object: Ws,
     get_spread_update: Ns,
     group_outros: Us,
     init: js,
-    insert: Ze,
+    insert: Qe,
     mount_component: tt,
     safe_not_equal: zs,
     set_data: qs,
-    space: Bt,
+    space: At,
     text: Ks,
-    transition_in: Ee,
-    transition_out: Oe
+    transition_in: Le,
+    transition_out: Pe
 } = window.__gradio__svelte__internal, {
     onMount: Vs
 } = window.__gradio__svelte__internal;
 
-function Tt(E) {
-    let m, S;
+function Bt(E) {
+    let f, p;
     const y = [{
             autoscroll: (
                 /*gradio*/
                 E[0].autoscroll
             )
         }, {
             i18n: (
                 /*gradio*/
                 E[0].i18n
             )
         },
         /*loading_status*/
         E[9]
     ];
-    let R = {};
+    let D = {};
     for (let M = 0; M < y.length; M += 1)
-        R = Is(R, y[M]);
-    return m = new Bs({
-        props: R
+        D = Is(D, y[M]);
+    return f = new As({
+        props: D
     }), {
         c() {
-            Qe(m.$$.fragment);
+            $e(f.$$.fragment);
         },
         m(M, k) {
-            tt(m, M, k), S = !0;
+            tt(f, M, k), p = !0;
         },
         p(M, k) {
-            const i = k & /*gradio, loading_status*/
+            const i = k[0] & /*gradio, loading_status*/
                 513 ? Ns(y, [
-                    k & /*gradio*/
+                    k[0] & /*gradio*/
                     1 && {
                         autoscroll: (
                             /*gradio*/
                             M[0].autoscroll
                         )
                     },
-                    k & /*gradio*/
+                    k[0] & /*gradio*/
                     1 && {
                         i18n: (
                             /*gradio*/
                             M[0].i18n
                         )
                     },
-                    k & /*loading_status*/
+                    k[0] & /*loading_status*/
                     512 && Ws(
                         /*loading_status*/
                         M[9]
                     )
                 ]) : {};
-            m.$set(i);
+            f.$set(i);
         },
         i(M) {
-            S || (Ee(m.$$.fragment, M), S = !0);
+            p || (Le(f.$$.fragment, M), p = !0);
         },
         o(M) {
-            Oe(m.$$.fragment, M), S = !1;
+            Pe(f.$$.fragment, M), p = !1;
         },
         d(M) {
-            et(m, M);
+            et(f, M);
         }
     };
 }
 
 function Gs(E) {
-    let m;
+    let f;
     return {
         c() {
-            m = Ks(
+            f = Ks(
                 /*label*/
                 E[1]
             );
         },
-        m(S, y) {
-            Ze(S, m, y);
+        m(p, y) {
+            Qe(p, f, y);
         },
-        p(S, y) {
-            y & /*label*/
+        p(p, y) {
+            y[0] & /*label*/
                 2 && qs(
-                    m,
+                    f,
                     /*label*/
-                    S[1]
+                    p[1]
                 );
         },
-        d(S) {
-            S && Ye(m);
+        d(p) {
+            p && Ze(f);
         }
     };
 }
 
 function Xs(E) {
-    let m, S, y, R, M, k, i = (
+    let f, p, y, D, M, k, i = (
         /*loading_status*/
-        E[9] && Tt(E)
+        E[9] && Bt(E)
     );
     return y = new zi({
         props: {
             show_label: (
                 /*show_label*/
                 E[6]
             ),
@@ -10941,49 +10941,50 @@
             },
             $$scope: {
                 ctx: E
             }
         }
     }), {
         c() {
-            i && i.c(), m = Bt(), S = At("div"), Qe(y.$$.fragment), R = Bt(), M = At("div"), Rt(M, "class", "svelte-1jxdgz3"), Rt(S, "class", "svelte-1jxdgz3");
+            i && i.c(), f = At(), p = Rt("div"), $e(y.$$.fragment), D = At(), M = Rt("div"), Dt(M, "class", "svelte-1jxdgz3"), Dt(p, "class", "svelte-1jxdgz3");
         },
         m(n, o) {
-            i && i.m(n, o), Ze(n, m, o), Ze(n, S, o), tt(y, S, null), Dt(S, R), Dt(S, M), E[14](M), k = !0;
+            i && i.m(n, o), Qe(n, f, o), Qe(n, p, o), tt(y, p, null), xt(p, D), xt(p, M), E[49](M), k = !0;
         },
         p(n, o) {
             /*loading_status*/
-            n[9] ? i ? (i.p(n, o), o & /*loading_status*/
-                512 && Ee(i, 1)) : (i = Tt(n), i.c(), Ee(i, 1), i.m(m.parentNode, m)) : i && (Us(), Oe(i, 1, 1, () => {
+            n[9] ? i ? (i.p(n, o), o[0] & /*loading_status*/
+                512 && Le(i, 1)) : (i = Bt(n), i.c(), Le(i, 1), i.m(f.parentNode, f)) : i && (Us(), Pe(i, 1, 1, () => {
                 i = null;
             }), Fs());
             const c = {};
-            o & /*show_label*/
+            o[0] & /*show_label*/
                 64 && (c.show_label = /*show_label*/
-                    n[6]), o & /*$$scope, label*/
-                65538 && (c.$$scope = {
+                    n[6]), o[0] & /*label*/
+                2 | o[1] & /*$$scope*/
+                1048576 && (c.$$scope = {
                     dirty: o,
                     ctx: n
                 }), y.$set(c);
         },
         i(n) {
-            k || (Ee(i), Ee(y.$$.fragment, n), k = !0);
+            k || (Le(i), Le(y.$$.fragment, n), k = !0);
         },
         o(n) {
-            Oe(i), Oe(y.$$.fragment, n), k = !1;
+            Pe(i), Pe(y.$$.fragment, n), k = !1;
         },
         d(n) {
-            n && (Ye(m), Ye(S)), i && i.d(n), et(y), E[14](null);
+            n && (Ze(f), Ze(p)), i && i.d(n), et(y), E[49](null);
         }
     };
 }
 
 function Js(E) {
-    let m, S;
-    return m = new oi({
+    let f, p;
+    return f = new oi({
         props: {
             visible: (
                 /*visible*/
                 E[5]
             ),
             elem_id: (
                 /*elem_id*/
@@ -11010,253 +11011,758 @@
             },
             $$scope: {
                 ctx: E
             }
         }
     }), {
         c() {
-            Qe(m.$$.fragment);
+            $e(f.$$.fragment);
         },
-        m(y, R) {
-            tt(m, y, R), S = !0;
+        m(y, D) {
+            tt(f, y, D), p = !0;
         },
-        p(y, [R]) {
+        p(y, D) {
             const M = {};
-            R & /*visible*/
+            D[0] & /*visible*/
                 32 && (M.visible = /*visible*/
-                    y[5]), R & /*elem_id*/
+                    y[5]), D[0] & /*elem_id*/
                 8 && (M.elem_id = /*elem_id*/
-                    y[3]), R & /*scale*/
+                    y[3]), D[0] & /*scale*/
                 128 && (M.scale = /*scale*/
-                    y[7]), R & /*min_width*/
+                    y[7]), D[0] & /*min_width*/
                 256 && (M.min_width = /*min_width*/
-                    y[8]), R & /*elem_classes, dark*/
+                    y[8]), D[0] & /*elem_classes, dark*/
                 20 && (M.elem_classes = [
                     ... /*elem_classes*/
                     y[4],
                     /*dark*/
                     y[2] ? "dark" : ""
-                ]), R & /*$$scope, termNode, show_label, label, gradio, loading_status*/
-                67139 && (M.$$scope = {
-                    dirty: R,
+                ]), D[0] & /*termNode, show_label, label, gradio, loading_status*/
+                1603 | D[1] & /*$$scope*/
+                1048576 && (M.$$scope = {
+                    dirty: D,
                     ctx: y
-                }), m.$set(M);
+                }), f.$set(M);
         },
         i(y) {
-            S || (Ee(m.$$.fragment, y), S = !0);
+            p || (Le(f.$$.fragment, y), p = !0);
         },
         o(y) {
-            Oe(m.$$.fragment, y), S = !1;
+            Pe(f.$$.fragment, y), p = !1;
         },
         d(y) {
-            et(m, y);
+            et(f, y);
         }
     };
 }
 
-function $s(E, m, S) {
+function Ys(E, f, p) {
     let y, {
-            gradio: R
-        } = m,
+            gradio: D
+        } = f,
         {
             log_file: M = ""
-        } = m,
+        } = f,
         {
             label: k = `log of ${M}`
-        } = m,
+        } = f,
         {
             dark: i = !1
-        } = m,
+        } = f,
         {
             elem_id: n = ""
-        } = m,
+        } = f,
         {
             elem_classes: o = ["terminal-block"]
-        } = m,
+        } = f,
         {
             visible: c = !0
-        } = m,
+        } = f,
         {
             value: a = ""
-        } = m,
+        } = f,
         {
             show_label: d
-        } = m,
+        } = f,
         {
-            scale: f = null
-        } = m,
+            scale: v = null
+        } = f,
         {
-            min_width: g = void 0
-        } = m,
+            min_width: m = void 0
+        } = f,
         {
             loading_status: l = void 0
-        } = m,
-        s, r;
+        } = f,
+        {
+            xterm_allow_proposed_api: s
+        } = f,
+        {
+            xterm_allow_transparency: r
+        } = f,
+        {
+            xterm_alt_click_moves_cursor: e
+        } = f,
+        {
+            xterm_convert_eol: t
+        } = f,
+        {
+            xterm_cursor_blink: h
+        } = f,
+        {
+            xterm_cursor_inactive_style: g
+        } = f,
+        {
+            xterm_cursor_style: u
+        } = f,
+        {
+            xterm_cursor_width: S
+        } = f,
+        {
+            xterm_custom_glyphs: _
+        } = f,
+        {
+            xterm_disable_stdin: b
+        } = f,
+        {
+            xterm_document_override: R
+        } = f,
+        {
+            xterm_draw_bold_text_in_bright_colors: B
+        } = f,
+        {
+            xterm_fast_scroll_modifier: T
+        } = f,
+        {
+            xterm_fast_scroll_sensitivity: L
+        } = f,
+        {
+            xterm_font_family: H
+        } = f,
+        {
+            xterm_font_size: W
+        } = f,
+        {
+            xterm_font_weight: j
+        } = f,
+        {
+            xterm_font_weight_bold: V
+        } = f,
+        {
+            xterm_ignore_bracketed_paste_mode: z
+        } = f,
+        {
+            xterm_letter_spacing: C
+        } = f,
+        {
+            xterm_line_height: x
+        } = f,
+        {
+            xterm_log_level: A
+        } = f,
+        {
+            xterm_mac_option_click_forces_selection: O
+        } = f,
+        {
+            xterm_mac_option_is_meta: I
+        } = f,
+        {
+            xterm_minimum_contrast_ratio: q
+        } = f,
+        {
+            xterm_overview_ruler_width: X
+        } = f,
+        {
+            xterm_rescale_overlapping_glyphs: J
+        } = f,
+        {
+            xterm_right_click_selects_word: P
+        } = f,
+        {
+            xterm_screen_reader_mode: w
+        } = f,
+        {
+            xterm_scroll_on_user_input: U
+        } = f,
+        {
+            xterm_scroll_sensitivity: F
+        } = f,
+        {
+            xterm_scrollback: G
+        } = f,
+        {
+            xterm_smooth_scroll_duration: K
+        } = f,
+        {
+            xterm_tab_stop_width: ee
+        } = f,
+        {
+            xterm_windows_mode: se
+        } = f,
+        ie, oe;
     Vs(() => {
-        S(13, s = new Ms.Terminal({
-            // allowTransparency: true,
-            theme: y
-        })), s.open(r);
-        const e = new Os.FitAddon();
-        s.loadAddon(e), setTimeout(
+        p(48, ie = new Ms.Terminal({
+            theme: y,
+            allowProposedApi: s,
+            allowTransparency: r,
+            altClickMovesCursor: e,
+            convertEol: t,
+            cursorBlink: h,
+            cursorInactiveStyle: g,
+            cursorStyle: u,
+            cursorWidth: S,
+            customGlyphs: _,
+            disableStdin: b,
+            documentOverride: R,
+            drawBoldTextInBrightColors: B,
+            fastScrollModifier: T,
+            fastScrollSensitivity: L,
+            fontFamily: H,
+            fontSize: W,
+            fontWeight: j,
+            fontWeightBold: V,
+            ignoreBracketedPasteMode: z,
+            letterSpacing: C,
+            lineHeight: x,
+            logLevel: A,
+            macOptionClickForcesSelection: O,
+            macOptionIsMeta: I,
+            minimumContrastRatio: q,
+            overviewRulerWidth: X,
+            rescaleOverlappingGlyphs: J,
+            rightClickSelectsWord: P,
+            screenReaderMode: w,
+            scrollOnUserInput: U,
+            scrollSensitivity: F,
+            smoothScrollDuration: K,
+            tabStopWidth: ee,
+            scrollback: G,
+            windowsMode: se
+        })), ie.open(oe);
+        const N = new Os.FitAddon();
+        ie.loadAddon(N), setTimeout(
             () => {
-                e.fit();
+                N.fit();
             },
             300
         );
+        const we = () => {
+            N.fit();
+        };
+        return window.addEventListener("resize", we), () => {
+            window.removeEventListener("resize", we);
+        };
     });
 
-    function t(e) {
-        Hs[e ? "unshift" : "push"](() => {
-            r = e, S(10, r);
+    function Z(N) {
+        Hs[N ? "unshift" : "push"](() => {
+            oe = N, p(10, oe);
         });
     }
-    return E.$$set = (e) => {
-        "gradio" in e && S(0, R = e.gradio), "log_file" in e && S(11, M = e.log_file), "label" in e && S(1, k = e.label), "dark" in e && S(2, i = e.dark), "elem_id" in e && S(3, n = e.elem_id), "elem_classes" in e && S(4, o = e.elem_classes), "visible" in e && S(5, c = e.visible), "value" in e && S(12, a = e.value), "show_label" in e && S(6, d = e.show_label), "scale" in e && S(7, f = e.scale), "min_width" in e && S(8, g = e.min_width), "loading_status" in e && S(9, l = e.loading_status);
+    return E.$$set = (N) => {
+        "gradio" in N && p(0, D = N.gradio), "log_file" in N && p(11, M = N.log_file), "label" in N && p(1, k = N.label), "dark" in N && p(2, i = N.dark), "elem_id" in N && p(3, n = N.elem_id), "elem_classes" in N && p(4, o = N.elem_classes), "visible" in N && p(5, c = N.visible), "value" in N && p(12, a = N.value), "show_label" in N && p(6, d = N.show_label), "scale" in N && p(7, v = N.scale), "min_width" in N && p(8, m = N.min_width), "loading_status" in N && p(9, l = N.loading_status), "xterm_allow_proposed_api" in N && p(13, s = N.xterm_allow_proposed_api), "xterm_allow_transparency" in N && p(14, r = N.xterm_allow_transparency), "xterm_alt_click_moves_cursor" in N && p(15, e = N.xterm_alt_click_moves_cursor), "xterm_convert_eol" in N && p(16, t = N.xterm_convert_eol), "xterm_cursor_blink" in N && p(17, h = N.xterm_cursor_blink), "xterm_cursor_inactive_style" in N && p(18, g = N.xterm_cursor_inactive_style), "xterm_cursor_style" in N && p(19, u = N.xterm_cursor_style), "xterm_cursor_width" in N && p(20, S = N.xterm_cursor_width), "xterm_custom_glyphs" in N && p(21, _ = N.xterm_custom_glyphs), "xterm_disable_stdin" in N && p(22, b = N.xterm_disable_stdin), "xterm_document_override" in N && p(23, R = N.xterm_document_override), "xterm_draw_bold_text_in_bright_colors" in N && p(24, B = N.xterm_draw_bold_text_in_bright_colors), "xterm_fast_scroll_modifier" in N && p(25, T = N.xterm_fast_scroll_modifier), "xterm_fast_scroll_sensitivity" in N && p(26, L = N.xterm_fast_scroll_sensitivity), "xterm_font_family" in N && p(27, H = N.xterm_font_family), "xterm_font_size" in N && p(28, W = N.xterm_font_size), "xterm_font_weight" in N && p(29, j = N.xterm_font_weight), "xterm_font_weight_bold" in N && p(30, V = N.xterm_font_weight_bold), "xterm_ignore_bracketed_paste_mode" in N && p(31, z = N.xterm_ignore_bracketed_paste_mode), "xterm_letter_spacing" in N && p(32, C = N.xterm_letter_spacing), "xterm_line_height" in N && p(33, x = N.xterm_line_height), "xterm_log_level" in N && p(34, A = N.xterm_log_level), "xterm_mac_option_click_forces_selection" in N && p(35, O = N.xterm_mac_option_click_forces_selection), "xterm_mac_option_is_meta" in N && p(36, I = N.xterm_mac_option_is_meta), "xterm_minimum_contrast_ratio" in N && p(37, q = N.xterm_minimum_contrast_ratio), "xterm_overview_ruler_width" in N && p(38, X = N.xterm_overview_ruler_width), "xterm_rescale_overlapping_glyphs" in N && p(39, J = N.xterm_rescale_overlapping_glyphs), "xterm_right_click_selects_word" in N && p(40, P = N.xterm_right_click_selects_word), "xterm_screen_reader_mode" in N && p(41, w = N.xterm_screen_reader_mode), "xterm_scroll_on_user_input" in N && p(42, U = N.xterm_scroll_on_user_input), "xterm_scroll_sensitivity" in N && p(43, F = N.xterm_scroll_sensitivity), "xterm_scrollback" in N && p(44, G = N.xterm_scrollback), "xterm_smooth_scroll_duration" in N && p(45, K = N.xterm_smooth_scroll_duration), "xterm_tab_stop_width" in N && p(46, ee = N.xterm_tab_stop_width), "xterm_windows_mode" in N && p(47, se = N.xterm_windows_mode);
     }, E.$$.update = () => {
-        E.$$.dirty & /*dark*/
+        E.$$.dirty[0] & /*dark*/
             4 && (y = i ? {
                 foreground: "white",
                 background: "#1F2937"
             } : {
                 foreground: "#1F2937",
                 background: "white",
                 selectionBackground: "#e5e7eb"
-            }), E.$$.dirty & /*term, value*/
-            12288 && s && a && a.trim() !== "" && s.write(a.replace(/\n/g, `
+            }), E.$$.dirty[0] & /*value*/
+            4096 | E.$$.dirty[1] & /*term*/
+            131072 && ie && a && a.trim() !== "" && ie.write(a.replace(/\n/g, `
 \r`));
     }, [
-        R,
+        D,
         k,
         i,
         n,
         o,
         c,
         d,
-        f,
-        g,
+        v,
+        m,
         l,
-        r,
+        oe,
         M,
         a,
         s,
-        t
+        r,
+        e,
+        t,
+        h,
+        g,
+        u,
+        S,
+        _,
+        b,
+        R,
+        B,
+        T,
+        L,
+        H,
+        W,
+        j,
+        V,
+        z,
+        C,
+        x,
+        A,
+        O,
+        I,
+        q,
+        X,
+        J,
+        P,
+        w,
+        U,
+        F,
+        G,
+        K,
+        ee,
+        se,
+        ie,
+        Z
     ];
 }
-class Ys extends Ps {
-    constructor(m) {
-        super(), js(this, m, $s, Js, zs, {
-            gradio: 0,
-            log_file: 11,
-            label: 1,
-            dark: 2,
-            elem_id: 3,
-            elem_classes: 4,
-            visible: 5,
-            value: 12,
-            show_label: 6,
-            scale: 7,
-            min_width: 8,
-            loading_status: 9
-        });
+class Zs extends Ps {
+    constructor(f) {
+        super(), js(
+            this,
+            f,
+            Ys,
+            Js,
+            zs, {
+                gradio: 0,
+                log_file: 11,
+                label: 1,
+                dark: 2,
+                elem_id: 3,
+                elem_classes: 4,
+                visible: 5,
+                value: 12,
+                show_label: 6,
+                scale: 7,
+                min_width: 8,
+                loading_status: 9,
+                xterm_allow_proposed_api: 13,
+                xterm_allow_transparency: 14,
+                xterm_alt_click_moves_cursor: 15,
+                xterm_convert_eol: 16,
+                xterm_cursor_blink: 17,
+                xterm_cursor_inactive_style: 18,
+                xterm_cursor_style: 19,
+                xterm_cursor_width: 20,
+                xterm_custom_glyphs: 21,
+                xterm_disable_stdin: 22,
+                xterm_document_override: 23,
+                xterm_draw_bold_text_in_bright_colors: 24,
+                xterm_fast_scroll_modifier: 25,
+                xterm_fast_scroll_sensitivity: 26,
+                xterm_font_family: 27,
+                xterm_font_size: 28,
+                xterm_font_weight: 29,
+                xterm_font_weight_bold: 30,
+                xterm_ignore_bracketed_paste_mode: 31,
+                xterm_letter_spacing: 32,
+                xterm_line_height: 33,
+                xterm_log_level: 34,
+                xterm_mac_option_click_forces_selection: 35,
+                xterm_mac_option_is_meta: 36,
+                xterm_minimum_contrast_ratio: 37,
+                xterm_overview_ruler_width: 38,
+                xterm_rescale_overlapping_glyphs: 39,
+                xterm_right_click_selects_word: 40,
+                xterm_screen_reader_mode: 41,
+                xterm_scroll_on_user_input: 42,
+                xterm_scroll_sensitivity: 43,
+                xterm_scrollback: 44,
+                xterm_smooth_scroll_duration: 45,
+                xterm_tab_stop_width: 46,
+                xterm_windows_mode: 47
+            },
+            null,
+            [-1, -1]
+        );
     }
     get gradio() {
         return this.$$.ctx[0];
     }
-    set gradio(m) {
+    set gradio(f) {
         this.$$set({
-            gradio: m
-        }), ae();
+            gradio: f
+        }), Y();
     }
     get log_file() {
         return this.$$.ctx[11];
     }
-    set log_file(m) {
+    set log_file(f) {
         this.$$set({
-            log_file: m
-        }), ae();
+            log_file: f
+        }), Y();
     }
     get label() {
         return this.$$.ctx[1];
     }
-    set label(m) {
+    set label(f) {
         this.$$set({
-            label: m
-        }), ae();
+            label: f
+        }), Y();
     }
     get dark() {
         return this.$$.ctx[2];
     }
-    set dark(m) {
+    set dark(f) {
         this.$$set({
-            dark: m
-        }), ae();
+            dark: f
+        }), Y();
     }
     get elem_id() {
         return this.$$.ctx[3];
     }
-    set elem_id(m) {
+    set elem_id(f) {
         this.$$set({
-            elem_id: m
-        }), ae();
+            elem_id: f
+        }), Y();
     }
     get elem_classes() {
         return this.$$.ctx[4];
     }
-    set elem_classes(m) {
+    set elem_classes(f) {
         this.$$set({
-            elem_classes: m
-        }), ae();
+            elem_classes: f
+        }), Y();
     }
     get visible() {
         return this.$$.ctx[5];
     }
-    set visible(m) {
+    set visible(f) {
         this.$$set({
-            visible: m
-        }), ae();
+            visible: f
+        }), Y();
     }
     get value() {
         return this.$$.ctx[12];
     }
-    set value(m) {
+    set value(f) {
         this.$$set({
-            value: m
-        }), ae();
+            value: f
+        }), Y();
     }
     get show_label() {
         return this.$$.ctx[6];
     }
-    set show_label(m) {
+    set show_label(f) {
         this.$$set({
-            show_label: m
-        }), ae();
+            show_label: f
+        }), Y();
     }
     get scale() {
         return this.$$.ctx[7];
     }
-    set scale(m) {
+    set scale(f) {
         this.$$set({
-            scale: m
-        }), ae();
+            scale: f
+        }), Y();
     }
     get min_width() {
         return this.$$.ctx[8];
     }
-    set min_width(m) {
+    set min_width(f) {
         this.$$set({
-            min_width: m
-        }), ae();
+            min_width: f
+        }), Y();
     }
     get loading_status() {
         return this.$$.ctx[9];
     }
-    set loading_status(m) {
+    set loading_status(f) {
+        this.$$set({
+            loading_status: f
+        }), Y();
+    }
+    get xterm_allow_proposed_api() {
+        return this.$$.ctx[13];
+    }
+    set xterm_allow_proposed_api(f) {
+        this.$$set({
+            xterm_allow_proposed_api: f
+        }), Y();
+    }
+    get xterm_allow_transparency() {
+        return this.$$.ctx[14];
+    }
+    set xterm_allow_transparency(f) {
+        this.$$set({
+            xterm_allow_transparency: f
+        }), Y();
+    }
+    get xterm_alt_click_moves_cursor() {
+        return this.$$.ctx[15];
+    }
+    set xterm_alt_click_moves_cursor(f) {
+        this.$$set({
+            xterm_alt_click_moves_cursor: f
+        }), Y();
+    }
+    get xterm_convert_eol() {
+        return this.$$.ctx[16];
+    }
+    set xterm_convert_eol(f) {
+        this.$$set({
+            xterm_convert_eol: f
+        }), Y();
+    }
+    get xterm_cursor_blink() {
+        return this.$$.ctx[17];
+    }
+    set xterm_cursor_blink(f) {
+        this.$$set({
+            xterm_cursor_blink: f
+        }), Y();
+    }
+    get xterm_cursor_inactive_style() {
+        return this.$$.ctx[18];
+    }
+    set xterm_cursor_inactive_style(f) {
+        this.$$set({
+            xterm_cursor_inactive_style: f
+        }), Y();
+    }
+    get xterm_cursor_style() {
+        return this.$$.ctx[19];
+    }
+    set xterm_cursor_style(f) {
+        this.$$set({
+            xterm_cursor_style: f
+        }), Y();
+    }
+    get xterm_cursor_width() {
+        return this.$$.ctx[20];
+    }
+    set xterm_cursor_width(f) {
+        this.$$set({
+            xterm_cursor_width: f
+        }), Y();
+    }
+    get xterm_custom_glyphs() {
+        return this.$$.ctx[21];
+    }
+    set xterm_custom_glyphs(f) {
+        this.$$set({
+            xterm_custom_glyphs: f
+        }), Y();
+    }
+    get xterm_disable_stdin() {
+        return this.$$.ctx[22];
+    }
+    set xterm_disable_stdin(f) {
+        this.$$set({
+            xterm_disable_stdin: f
+        }), Y();
+    }
+    get xterm_document_override() {
+        return this.$$.ctx[23];
+    }
+    set xterm_document_override(f) {
+        this.$$set({
+            xterm_document_override: f
+        }), Y();
+    }
+    get xterm_draw_bold_text_in_bright_colors() {
+        return this.$$.ctx[24];
+    }
+    set xterm_draw_bold_text_in_bright_colors(f) {
+        this.$$set({
+            xterm_draw_bold_text_in_bright_colors: f
+        }), Y();
+    }
+    get xterm_fast_scroll_modifier() {
+        return this.$$.ctx[25];
+    }
+    set xterm_fast_scroll_modifier(f) {
+        this.$$set({
+            xterm_fast_scroll_modifier: f
+        }), Y();
+    }
+    get xterm_fast_scroll_sensitivity() {
+        return this.$$.ctx[26];
+    }
+    set xterm_fast_scroll_sensitivity(f) {
+        this.$$set({
+            xterm_fast_scroll_sensitivity: f
+        }), Y();
+    }
+    get xterm_font_family() {
+        return this.$$.ctx[27];
+    }
+    set xterm_font_family(f) {
+        this.$$set({
+            xterm_font_family: f
+        }), Y();
+    }
+    get xterm_font_size() {
+        return this.$$.ctx[28];
+    }
+    set xterm_font_size(f) {
+        this.$$set({
+            xterm_font_size: f
+        }), Y();
+    }
+    get xterm_font_weight() {
+        return this.$$.ctx[29];
+    }
+    set xterm_font_weight(f) {
+        this.$$set({
+            xterm_font_weight: f
+        }), Y();
+    }
+    get xterm_font_weight_bold() {
+        return this.$$.ctx[30];
+    }
+    set xterm_font_weight_bold(f) {
+        this.$$set({
+            xterm_font_weight_bold: f
+        }), Y();
+    }
+    get xterm_ignore_bracketed_paste_mode() {
+        return this.$$.ctx[31];
+    }
+    set xterm_ignore_bracketed_paste_mode(f) {
+        this.$$set({
+            xterm_ignore_bracketed_paste_mode: f
+        }), Y();
+    }
+    get xterm_letter_spacing() {
+        return this.$$.ctx[32];
+    }
+    set xterm_letter_spacing(f) {
+        this.$$set({
+            xterm_letter_spacing: f
+        }), Y();
+    }
+    get xterm_line_height() {
+        return this.$$.ctx[33];
+    }
+    set xterm_line_height(f) {
+        this.$$set({
+            xterm_line_height: f
+        }), Y();
+    }
+    get xterm_log_level() {
+        return this.$$.ctx[34];
+    }
+    set xterm_log_level(f) {
+        this.$$set({
+            xterm_log_level: f
+        }), Y();
+    }
+    get xterm_mac_option_click_forces_selection() {
+        return this.$$.ctx[35];
+    }
+    set xterm_mac_option_click_forces_selection(f) {
+        this.$$set({
+            xterm_mac_option_click_forces_selection: f
+        }), Y();
+    }
+    get xterm_mac_option_is_meta() {
+        return this.$$.ctx[36];
+    }
+    set xterm_mac_option_is_meta(f) {
+        this.$$set({
+            xterm_mac_option_is_meta: f
+        }), Y();
+    }
+    get xterm_minimum_contrast_ratio() {
+        return this.$$.ctx[37];
+    }
+    set xterm_minimum_contrast_ratio(f) {
+        this.$$set({
+            xterm_minimum_contrast_ratio: f
+        }), Y();
+    }
+    get xterm_overview_ruler_width() {
+        return this.$$.ctx[38];
+    }
+    set xterm_overview_ruler_width(f) {
+        this.$$set({
+            xterm_overview_ruler_width: f
+        }), Y();
+    }
+    get xterm_rescale_overlapping_glyphs() {
+        return this.$$.ctx[39];
+    }
+    set xterm_rescale_overlapping_glyphs(f) {
+        this.$$set({
+            xterm_rescale_overlapping_glyphs: f
+        }), Y();
+    }
+    get xterm_right_click_selects_word() {
+        return this.$$.ctx[40];
+    }
+    set xterm_right_click_selects_word(f) {
+        this.$$set({
+            xterm_right_click_selects_word: f
+        }), Y();
+    }
+    get xterm_screen_reader_mode() {
+        return this.$$.ctx[41];
+    }
+    set xterm_screen_reader_mode(f) {
+        this.$$set({
+            xterm_screen_reader_mode: f
+        }), Y();
+    }
+    get xterm_scroll_on_user_input() {
+        return this.$$.ctx[42];
+    }
+    set xterm_scroll_on_user_input(f) {
+        this.$$set({
+            xterm_scroll_on_user_input: f
+        }), Y();
+    }
+    get xterm_scroll_sensitivity() {
+        return this.$$.ctx[43];
+    }
+    set xterm_scroll_sensitivity(f) {
+        this.$$set({
+            xterm_scroll_sensitivity: f
+        }), Y();
+    }
+    get xterm_scrollback() {
+        return this.$$.ctx[44];
+    }
+    set xterm_scrollback(f) {
+        this.$$set({
+            xterm_scrollback: f
+        }), Y();
+    }
+    get xterm_smooth_scroll_duration() {
+        return this.$$.ctx[45];
+    }
+    set xterm_smooth_scroll_duration(f) {
+        this.$$set({
+            xterm_smooth_scroll_duration: f
+        }), Y();
+    }
+    get xterm_tab_stop_width() {
+        return this.$$.ctx[46];
+    }
+    set xterm_tab_stop_width(f) {
+        this.$$set({
+            xterm_tab_stop_width: f
+        }), Y();
+    }
+    get xterm_windows_mode() {
+        return this.$$.ctx[47];
+    }
+    set xterm_windows_mode(f) {
         this.$$set({
-            loading_status: m
-        }), ae();
+            xterm_windows_mode: f
+        }), Y();
     }
 }
 export {
-    Ys as
+    Zs as
     default
 };
```

### Comparing `gradio_log-0.0.3/backend/gradio_log/templates/component/style.css` & `gradio_log-0.0.4/backend/gradio_log/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_log-0.0.3/demo/app.py` & `gradio_log-0.0.4/demo/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from pathlib import Path
 import logging
-import gradio as gr
+from pathlib import Path
 
+import gradio as gr
 from gradio_log import Log
 
-import logging
-
 
 class CustomFormatter(logging.Formatter):
 
     green = "\x1b[32;20m"
     blue = "\x1b[34;20m"
     yellow = "\x1b[33;20m"
     red = "\x1b[31;20m"
@@ -47,25 +45,24 @@
 logger.addHandler(ch)
 
 
 logger.info("The logs will be displayed in here.")
 
 
 def create_log_handler(level):
-
     def l(text):
         getattr(logger, level)(text)
 
     return l
 
 
 with gr.Blocks() as demo:
     text = gr.Textbox(label="Enter text to write to log file")
     with gr.Row():
         for l in ["debug", "info", "warning", "error", "critical"]:
             button = gr.Button(f"log as {l}")
             button.click(fn=create_log_handler(l), inputs=text)
-    Log(log_file)
+    Log(log_file, dark=True)
 
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_log-0.0.3/demo/css.css` & `gradio_log-0.0.4/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_log-0.0.3/frontend/package-lock.json` & `gradio_log-0.0.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_log-0.0.3/pyproject.toml` & `gradio_log-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_log"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Log component for Gradio which can easily show some log file in the interface."
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Chenglu", email = "chenglu.she@gmail.com" }]
 keywords = [
   "gradio-custom-component",
@@ -39,15 +39,15 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_log/templates", "*.pyi", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates"]
+artifacts = ["/backend/gradio_log/templates", "*.pyi", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates", "backend/gradio_log/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_log"]
 
 [project.urls]
 Homepage = "https://github.com/louis-she/gradio-log"
 Repository = "https://github.com/louis-she/gradio-log"
```

