# Comparing `tmp/ERA_V2_Architecture-0.1.3.tar.gz` & `tmp/ERA_V2_Architecture-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ERA_V2_Architecture-0.1.3.tar", last modified: Thu Apr 11 11:52:56 2024, max compression
+gzip compressed data, was "ERA_V2_Architecture-0.1.4.tar", last modified: Fri Apr 12 11:59:09 2024, max compression
```

## Comparing `ERA_V2_Architecture-0.1.3.tar` & `ERA_V2_Architecture-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:52:56.135841 ERA_V2_Architecture-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:52:56.094840 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/
--rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:52:56.127837 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/model/
--rw-rw-rw-   0        0        0      107 2024-04-11 11:51:53.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/model/__init__.py
--rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/model/models.py
--rw-rw-rw-   0        0        0     2915 2024-04-11 10:29:37.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/model/resnet.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:52:56.131837 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture.egg-info/
--rw-rw-rw-   0        0        0      473 2024-04-11 11:52:55.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-11 11:52:56.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:52:55.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-11 11:52:55.000000 ERA_V2_Architecture-0.1.3/ERA_V2_Architecture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-04-11 11:52:56.133839 ERA_V2_Architecture-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 11:52:56.135841 ERA_V2_Architecture-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-11 11:52:38.000000 ERA_V2_Architecture-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.496620 ERA_V2_Architecture-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.418750 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/
+-rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.480258 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/
+-rw-rw-rw-   0        0        0      107 2024-04-11 11:51:53.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/__init__.py
+-rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/models.py
+-rw-rw-rw-   0        0        0     3061 2024-04-12 11:56:27.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/resnet.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.480258 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      473 2024-04-12 11:59:09.494788 ERA_V2_Architecture-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 11:59:09.496620 ERA_V2_Architecture-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-04-12 11:56:39.000000 ERA_V2_Architecture-0.1.4/setup.py
```

### Comparing `ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/model/models.py` & `ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/models.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.3/ERA_V2_Architecture/model/resnet.py` & `ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/resnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,26 @@
         out = self.bn2(self.conv2(out))
         out += self.shortcut(x)
         out = F.relu(out)
         return out
 
 
 class ResNet(nn.Module):
-    def __init__(self, block, num_blocks, num_classes=10):
+    def __init__(self, block, num_blocks, num_classes=10):  
         super(ResNet, self).__init__()
         self.in_planes = 64
 
         self.conv1 = nn.Conv2d(3, 64, kernel_size=3,
                                stride=1, padding=1, bias=False)
         self.bn1 = nn.BatchNorm2d(64)
         self.layer1 = self._make_layer(block, 64, num_blocks[0], stride=1)
         self.layer2 = self._make_layer(block, 128, num_blocks[1], stride=2)
         self.layer3 = self._make_layer(block, 256, num_blocks[2], stride=2)
         self.layer4 = self._make_layer(block, 512, num_blocks[3], stride=2)
+        self.avgpool = nn.AdaptiveAvgPool2d((1, 1))  # Adaptive pooling to adjust pooling size automatically
         self.linear = nn.Linear(512*block.expansion, num_classes)
 
     def _make_layer(self, block, planes, num_blocks, stride):
         strides = [stride] + [1]*(num_blocks-1)
         layers = []
         for stride in strides:
             layers.append(block(self.in_planes, planes, stride))
@@ -63,15 +64,16 @@
 
     def forward(self, x):
         out = F.relu(self.bn1(self.conv1(x)))
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
-        out = F.avg_pool2d(out, 4)
+        #out = F.avg_pool2d(out, 4)
+        out = self.avgpool(out)
         out = out.view(out.size(0), -1)
         out = self.linear(out)
         return out
 
 
 def ResNet18():
     return ResNet(BasicBlock, [2, 2, 2, 2])
```

### Comparing `ERA_V2_Architecture-0.1.3/setup.py` & `ERA_V2_Architecture-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ERA_V2_Architecture",
-    version="0.1.3",
+    version="0.1.4",
     author="Xianping Wu",
     author_email="xianpingwu@hotmail.com",
     description="The ERA-V2 course network architectures",
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url="https://github.com/ping-Mel/ERAV2-Architecture.git",
     packages=find_packages(),
```

