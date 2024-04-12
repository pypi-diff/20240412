# Comparing `tmp/prusek_spheroid-5.0.tar.gz` & `tmp/prusek_spheroid-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-5.0.tar", last modified: Thu Apr 11 05:08:45 2024, max compression
+gzip compressed data, was "prusek_spheroid-5.1.tar", last modified: Fri Apr 12 12:15:01 2024, max compression
```

## Comparing `prusek_spheroid-5.0.tar` & `prusek_spheroid-5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-11 05:08:45.525872 prusek_spheroid-5.0/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9987 2024-04-11 05:08:45.525635 prusek_spheroid-5.0/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9415 2024-04-11 05:08:06.000000 prusek_spheroid-5.0/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-11 05:08:45.524400 prusek_spheroid-5.0/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-5.0/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    52496 2024-04-11 04:51:39.000000 prusek_spheroid-5.0/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.0/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.0/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.0/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-5.0/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.0/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.0/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.0/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.0/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.0/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-11 05:08:45.525429 prusek_spheroid-5.0/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9987 2024-04-11 05:08:45.000000 prusek_spheroid-5.0/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-11 05:08:45.000000 prusek_spheroid-5.0/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-11 05:08:45.000000 prusek_spheroid-5.0/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-11 05:08:45.000000 prusek_spheroid-5.0/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-11 05:08:45.000000 prusek_spheroid-5.0/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-11 05:08:45.525918 prusek_spheroid-5.0/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-11 05:08:26.000000 prusek_spheroid-5.0/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-12 12:15:01.394313 prusek_spheroid-5.1/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-12 12:15:01.394056 prusek_spheroid-5.1/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.1/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-12 12:15:01.393015 prusek_spheroid-5.1/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.1/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    52507 2024-04-12 12:01:36.000000 prusek_spheroid-5.1/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.1/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.1/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.1/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-5.1/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.1/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.1/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.1/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.1/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.1/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-12 12:15:01.393821 prusek_spheroid-5.1/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-12 12:15:01.394372 prusek_spheroid-5.1/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-12 12:14:58.000000 prusek_spheroid-5.1/setup.py
```

### Comparing `prusek_spheroid-5.0/PKG-INFO` & `prusek_spheroid-5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.0
+Version: 5.1
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -60,14 +60,19 @@
 1. **Activate your virtual environment** (if not already activated).
 2. **Install PyTorch** using pip by running the following command: `pip install torch`
 
 For specific versions and configurations (e.g., with CUDA support), visit the [PyTorch official website](https://pytorch.org/get-started/locally/) for the appropriate installation command.
 
 
 ## Running the Package
+Activate your Conda virtual environment using the command: `conda activate environment_name`
+
+Use the name of your created conda virtual environment instead of `environment_name`. 
+
+If you don't know the name, you can get it from the list of Conda virtual environments you've created using the command: `conda info --envs`
 
 To use the package, first ensure it is up to date: `pip install --upgrade prusek_spheroid`
 
 then run the program using the command: `python -m prusek_spheroid.GUI`
 
 ## Introductory window
 At the beginning, the user can choose which software he wants to use. There are two main ones to choose from. The first one is used to segment the spheroid images. It saves these segmentations and offers the possibility to determine the properties (quantify) of the spheroids based on these segmentations. The second option is used only to determine the properties of the spheroids based on the provided binary masks of the previously segmented spheroids. The other two ancillary software are image manipulation support programs. The first of these (left) is software for converting COCO 1.0 annotations to Masks, or the other way around. The second software is used to consolidate multiple image folders into one. The software assumes that the input directory branches into multiple directories and that the end folders contain images in BMP format. The software unifies these images from the end folders into one, changes their names to match the location in the directories, and removes duplicate images.
```

### Comparing `prusek_spheroid-5.0/README.md` & `prusek_spheroid-5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 1. **Activate your virtual environment** (if not already activated).
 2. **Install PyTorch** using pip by running the following command: `pip install torch`
 
 For specific versions and configurations (e.g., with CUDA support), visit the [PyTorch official website](https://pytorch.org/get-started/locally/) for the appropriate installation command.
 
 
 ## Running the Package
+Activate your Conda virtual environment using the command: `conda activate environment_name`
+
+Use the name of your created conda virtual environment instead of `environment_name`. 
+
+If you don't know the name, you can get it from the list of Conda virtual environments you've created using the command: `conda info --envs`
 
 To use the package, first ensure it is up to date: `pip install --upgrade prusek_spheroid`
 
 then run the program using the command: `python -m prusek_spheroid.GUI`
 
 ## Introductory window
 At the beginning, the user can choose which software he wants to use. There are two main ones to choose from. The first one is used to segment the spheroid images. It saves these segmentations and offers the possibility to determine the properties (quantify) of the spheroids based on these segmentations. The second option is used only to determine the properties of the spheroids based on the provided binary masks of the previously segmented spheroids. The other two ancillary software are image manipulation support programs. The first of these (left) is software for converting COCO 1.0 annotations to Masks, or the other way around. The second software is used to consolidate multiple image folders into one. The software assumes that the input directory branches into multiple directories and that the end folders contain images in BMP format. The software unifies these images from the end folders into one, changes their names to match the location in the directories, and removes duplicate images.
```

### Comparing `prusek_spheroid-5.0/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-5.1/prusek_spheroid/ContoursClassGUI.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,20 @@
                  contours_state, detect_corrupted, create_json, calculate_properties,
                  progress_window=None):
         super().__init__()
         self.counter = None
         self.master = master
         self.user_decision_lock = Lock()
         self.adresaDatasetu = adresaDatasetu
-        self.output_json_path = f"{adresa_output}/{projekt}/CVAT/{algorithm}/annotations/instances_default.json"
-        self.output_images_path = f"{adresa_output}/{projekt}/CVAT/{algorithm}/images"
-        self.output_segmented_path = f"{adresa_output}/{projekt}/segmented_images/{algorithm}"
-        self.zipfile_address = f"{adresa_output}/{projekt}/CVAT/{algorithm}"
-        self.excel_address = f"{adresa_output}/{projekt}"
+        self.output_json_path = os.path.join(adresa_output, projekt, "CVAT", algorithm, "annotations",
+                                             "instances_default.json")
+        self.output_images_path = os.path.join(adresa_output, projekt, "CVAT", algorithm, "images")
+        self.output_segmented_path = os.path.join(adresa_output, projekt, "segmented_images", algorithm)
+        self.zipfile_address = os.path.join(adresa_output, projekt, "CVAT", algorithm)
+        self.excel_address = os.path.join(adresa_output, projekt)
         self.coco_data = fm.initialize_coco_data()
         self.show_img = show_img
         self.projekt = projekt
         self.algorithm = algorithm
         self.parameters = parameters
         self.contours_state = contours_state
         self.detect_corrupted = detect_corrupted
@@ -50,24 +51,23 @@
             self.model = joblib.load(model_path)
             self.scaler = joblib.load(scaler_path)
         except Exception as e:
             print(f"Loading from primary location failed: {e}")
             print("Attempting to load from alternate location...")
             # Attempt to load the model and scaler from the alternate location
             # Load the model and scaler
-            model_path = os.path.join(current_dir, 'prusek_spheroid','gradient_boosting_classifier.joblib')
+            model_path = os.path.join(current_dir, 'prusek_spheroid', 'gradient_boosting_classifier.joblib')
             scaler_path = os.path.join(current_dir, 'prusek_spheroid', 'scaler.joblib')
             self.model = joblib.load(model_path)
             self.scaler = joblib.load(scaler_path)
 
-
         fm.create_directory(os.path.dirname(self.output_json_path), delete=True)
         fm.create_directory(self.output_images_path, delete=True)
-        fm.create_directory(f"{self.output_segmented_path}/masks", delete=True)
-        fm.create_directory(f"{self.output_segmented_path}/results", delete=True)
+        fm.create_directory(os.path.join(self.output_segmented_path, "masks"), delete=True)
+        fm.create_directory(os.path.join(self.output_segmented_path, "results"), delete=True)
 
     def evaluate(self, contour):
         hu_moments = ip.compute_hu_moments(contour)
         hu_moments_scaled = self.scaler.transform([hu_moments])
         contour_class = self.model.predict(hu_moments_scaled)[0]
         return contour_class
 
@@ -107,36 +107,35 @@
                 if self.contours_state == "all" or self.contours_state == "select":
                     inner_contours, _ = cv.findContours(inner_contours_mask, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
                     inner_contours = ip.remove_small_contours(inner_contours)
 
                 height, width = np.shape(img_binary)
 
                 outer_contours = ip.filter_contours_on_frame(outer_contours, (height, width), self.min_area,
-                                                                  self.detect_corrupted)
+                                                             self.detect_corrupted)
                 outer_contours = ip.remove_small_contours(outer_contours)
 
-
                 if self.create_json:
-                    if not cv.imwrite(f"{self.output_images_path}/{filename}", img):
-                        print(f"FAILED to save image: {self.output_images_path}/{filename}")
+                    if not cv.imwrite(os.path.join(self.output_images_path, filename), img):
+                        print(f"FAILED to save image: {os.path.join(self.output_images_path, filename)}")
 
                 img_with = img.copy()
                 if len(outer_contours) == 0:
                     if self.create_json:
                         self.coco_data = fm.convert_contours_to_coco([], [], height, width,
                                                                      filename,
                                                                      self.counter,
                                                                      self.coco_data)
                     cv.line(img_with, (0, 0), (width - 1, height - 1), (0, 0, 255), 5)
                     cv.line(img_with, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
                     if not cv.imwrite(
-                            f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
+                            os.path.join(self.output_segmented_path, "results", filename.replace('.bmp', '.png')),
                             img_with):
                         print(
-                            f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
+                            f"FAILED to save image: {os.path.join(self.output_segmented_path, 'results', filename.replace('.bmp', '.png'))}")
 
                 else:
                     img_without = img.copy()
                     mask_without = np.zeros_like(img_gray)
 
                     for contour in outer_contours:
                         contour = np.array(contour, dtype=np.int32)
@@ -149,63 +148,37 @@
                             cv.fillPoly(inner_mask, [contour], 255)
 
                         # Find intersection between outer and inner masks
                         intersection = mask_without & inner_mask
                         inner_contours, _ = cv.findContours(intersection, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
                         inner_contours = ip.remove_small_contours(inner_contours)
 
-
                         # Subtract intersection from the outer contours mask
                         mask_with = mask_without - intersection
 
                         for contour in inner_contours:
-                            cv.drawContours(img_with, [contour], -1, (255,0,0), 2)
-
+                            cv.drawContours(img_with, [contour], -1, (255, 0, 0), 2)
 
                     for index, contour in enumerate(outer_contours):
                         contour_budding = self.evaluate(contour)
 
                         if not contour_budding == "no_split":
-                            color = (0,255,0)
+                            color = (0, 255, 0)
                         else:
-                            color = (0,0,255)
+                            color = (0, 0, 255)
 
                         if self.contours_state == "all":
                             cv.drawContours(img_with, [contour], -1, color, 2)
                         elif self.contours_state == "no":
                             cv.drawContours(img_without, [contour], -1, color, 2)
                         else:
                             cv.drawContours(img_without, [contour], -1, color, 2)
                             cv.drawContours(img_with, [contour], -1, color, 2)
 
-                        if self.contours_state == "select" and dialog:
-                            dialog.update_selection_dialog(img_without, img_with, mask_without, mask_with,
-                                                           f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
-                                                           f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
-                                                           self.counter)
-                        elif self.contours_state == "all":
-                            if not cv.imwrite(f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
-                                              mask_with):
-                                print(
-                                    f"FAILED to save mask: {self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}")
-                            if not cv.imwrite(
-                                    f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
-                                    img_with):
-                                print(
-                                    f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
-                        else:
-                            if not cv.imwrite(f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
-                                              mask_without):
-                                print(
-                                    f"FAILED to save mask: {self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}")
-                            if not cv.imwrite(
-                                    f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
-                                    img_without):
-                                print(
-                                    f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
+                        self.save_images_and_masks(filename, (img_without, img_with, mask_without, mask_with), dialog)
 
                         if self.calculate_properties:
                             contour_data = {
                                 'MaskName': os.path.basename(filename),
                                 'ContourOrder': index + 1
                             }
 
@@ -237,43 +210,68 @@
             df = pd.DataFrame(all_contour_data, columns=[
                 'MaskName', 'ContourOrder', 'Area', 'Circularity', 'Compactness', 'Convexity',
                 'EquivalentDiameter', 'FeretAspectRatio', 'FeretDiameterMax',
                 'FeretDiameterMaxOrthogonalDistance', 'FeretDiameterMin',
                 'LengthMajorDiameterThroughCentroid', 'LengthMinorDiameterThroughCentroid',
                 'Perimeter', 'Solidity', 'Sphericity'
             ])
-            df.to_excel(f"{self.excel_address}/contour_properties.xlsx")
+            df.to_excel(os.path.join(self.excel_address, "contour_properties.xlsx"))
 
         if self.create_json:
             with open(self.output_json_path, "w") as json_file:
                 json.dump(self.coco_data, json_file)
             if self.progress_window:
                 self.progress_window.update_progress("zipping folder...")
             fm.zip_folder(self.zipfile_address, f"{self.zipfile_address}.zip")
 
         if self.progress_window:
             self.progress_window.update_progress("FINISHED")
 
+    def save_images_and_masks(self, filename, data, dialog=None):
+        img_without, img_with, mask_without, mask_with = data
+        # Construct the base paths for results and masks
+        results_path = os.path.join(self.output_segmented_path, "results")
+        masks_path = os.path.join(self.output_segmented_path, "masks")
+
+        # Replace the file extension from '.bmp' to '.png'
+        new_filename = f"{os.path.splitext(filename)[0]}.png"
+
+        # Full paths for the new image and mask files
+        new_image_path = os.path.join(results_path, new_filename)
+        new_mask_path = os.path.join(masks_path, new_filename)
+
+        if self.contours_state == "select" and dialog:
+            dialog.update_selection_dialog(img_without, img_with, mask_without, mask_with,
+                                           new_image_path, new_mask_path,
+                                           self.counter)
+        elif self.contours_state == "all":
+            if not cv.imwrite(new_mask_path, mask_with):
+                print(f"FAILED to save mask: {new_mask_path}")
+            if not cv.imwrite(new_image_path, img_with):
+                print(f"FAILED to save image: {new_image_path}")
+        else:
+            if not cv.imwrite(new_mask_path, mask_without):
+                print(f"FAILED to save mask: {new_mask_path}")
+            if not cv.imwrite(new_image_path, img_without):
+                print(f"FAILED to save image: {new_image_path}")
+
 
 class IoU(BaseImageProcessing):
     def __init__(self, adresa_output, project, algorithm, contours_state,
                  detect_corrupted):
         super().__init__()
         self.project = project
         self.algorithm = algorithm
         self.contours_state = contours_state
         self.detect_corrupted = detect_corrupted
-        self.adresa_output = f"{adresa_output}/{project}/IoU"
-        self.adresa_plots = f"{adresa_output}/{project}/IoU/plots/{self.algorithm}"
+        self.adresa_output = os.path.join(adresa_output, project, "IoU")
+        self.adresa_plots = os.path.join(self.adresa_output, "plots", self.algorithm)
 
         fm.create_directory(self.adresa_output)
 
-        # for mask, name in zip(self.masks, self.img_names):
-        #    cv.imwrite(f"img_print/{name}",mask)
-
     def process_and_compute_iou(self, ref_mask, img, img_name, parameters, save, lock):
         # Convert the mask tensor and image tensor to numpy arrays
         ref_mask = ref_mask.numpy()
         img = img.numpy()
 
         # Convert image to grayscale (assuming img is in BGR format)
         img_gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
@@ -285,15 +283,14 @@
         # Further processing and IoU, TPR, PPV computation
         if self.contours_state == "all" or self.contours_state == "select":
             intersection = inner_contours_mask & img_binary
             img_binary = img_binary - intersection
 
         contours, _ = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
 
-
         mask = np.zeros_like(img_binary, dtype=np.uint8)
         if not contours:
             # If no contours are found, draw a default contour
             contour = np.array([[0, 0]], dtype=np.int32)
             cv.drawContours(mask, [contour], 0, color=255, thickness=-1)
         else:
             # Draw contours on the mask
@@ -373,15 +370,15 @@
             contours_state_string = "WITH_HOLES"
         else:
             contours_state_string = "SELECT_HOLES"
 
         detect_corrupted_string = "WITH_detecting_corrupted" if self.detect_corrupted else "WITHOUT_detecting_corrupted"
 
         with open(
-                f"{self.adresa_output}/results_{self.project}_{self.algorithm}_IoU_{round(averageIoU * 100, 2)}_{contours_state_string}_{detect_corrupted_string}.json",
+                os.path.join(self.adresa_output, f"results_{self.project}_{self.algorithm}_IoU_{round(averageIoU * 100, 2)}_{contours_state_string}_{detect_corrupted_string}.json"),
                 "w") as json_file:
             json.dump(json_data, json_file, indent=4, cls=NumpyEncoder)
 
 
 def average_json_data(json_data_list):
     # Inicializujeme prázdné seznamy pro jednotlivé hodnoty
     parameters_list = []
```

### Comparing `prusek_spheroid-5.0/prusek_spheroid/GUI.py` & `prusek_spheroid-5.1/prusek_spheroid/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,15 +582,15 @@
             'EquivalentDiameter', 'FeretAspectRatio', 'FeretDiameterMax',
             'FeretDiameterMaxOrthogonalDistance', 'FeretDiameterMin',
             'LengthMajorDiameterThroughCentroid', 'LengthMinorDiameterThroughCentroid',
             'Perimeter', 'Solidity', 'Sphericity'
         ]
         df = pd.DataFrame(all_contour_data, columns=columns)
         output_path = self.output_path_quantification.get()
-        df.to_excel(f"{output_path}/contour_properties.xlsx")
+        df.to_excel(os.path.join(output_path,"contour_properties.xlsx"))
 
         # Close the progress dialog
         progress_dialog.destroy()
 
         # Show completion message
         messagebox.showinfo("Completed", f"Spheroid properties calculated and saved.\nOutput path: {output_path}")
         print("Spheroid properties calculated and saved.")
```

### Comparing `prusek_spheroid-5.0/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-5.1/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-5.1/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/conversion.py` & `prusek_spheroid-5.1/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/file_management.py` & `prusek_spheroid-5.1/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/image_processing.py` & `prusek_spheroid-5.1/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/merge_directories.py` & `prusek_spheroid-5.1/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/methods.py` & `prusek_spheroid-5.1/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/metrics.py` & `prusek_spheroid-5.1/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-5.1/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-5.1/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.0
+Version: 5.1
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -60,14 +60,19 @@
 1. **Activate your virtual environment** (if not already activated).
 2. **Install PyTorch** using pip by running the following command: `pip install torch`
 
 For specific versions and configurations (e.g., with CUDA support), visit the [PyTorch official website](https://pytorch.org/get-started/locally/) for the appropriate installation command.
 
 
 ## Running the Package
+Activate your Conda virtual environment using the command: `conda activate environment_name`
+
+Use the name of your created conda virtual environment instead of `environment_name`. 
+
+If you don't know the name, you can get it from the list of Conda virtual environments you've created using the command: `conda info --envs`
 
 To use the package, first ensure it is up to date: `pip install --upgrade prusek_spheroid`
 
 then run the program using the command: `python -m prusek_spheroid.GUI`
 
 ## Introductory window
 At the beginning, the user can choose which software he wants to use. There are two main ones to choose from. The first one is used to segment the spheroid images. It saves these segmentations and offers the possibility to determine the properties (quantify) of the spheroids based on these segmentations. The second option is used only to determine the properties of the spheroids based on the provided binary masks of the previously segmented spheroids. The other two ancillary software are image manipulation support programs. The first of these (left) is software for converting COCO 1.0 annotations to Masks, or the other way around. The second software is used to consolidate multiple image folders into one. The software assumes that the input directory branches into multiple directories and that the end folders contain images in BMP format. The software unifies these images from the end folders into one, changes their names to match the location in the directories, and removes duplicate images.
```

### Comparing `prusek_spheroid-5.0/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-5.1/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.0/setup.py` & `prusek_spheroid-5.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="5.0",
+    version="5.1",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

