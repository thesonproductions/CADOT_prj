# CADOT_prj

## Dataset

Data collected from the CADOT competition. The data is organized in the COCO (Common Objects in Context) format, a popular annotation format for object detection, segmentation, and captioning tasks.

### train

#### Overview

The training split (`# train`) comprises [**please fill in the number of images/samples in the training set**] images and their corresponding annotations for objects of interest within a CAD design context.

#### Data Format: COCO

The data adheres to the COCO format, which includes the following main components:

* **Images:** An array containing information about each image, including the image ID, width, height, and the path to the image file.
* **Annotations:** An array containing annotation information for each object instance in each image. Each annotation includes:
    * `id`: A unique ID for the annotation.
    * `image_id`: The ID of the image to which the object belongs.
    * `category_id`: The ID of the object category (class).
    * `segmentation`: Information about the object's boundary (typically a polygon).
    * `bbox`: The bounding box of the object in the format `[x_min, y_min, width, height]`.
    * `area`: The area of the segmented region.
    * `iscrowd`: A flag indicating if the object is a crowd of instances (0 if not, 1 if it is).
* **Categories:** An array containing information about the annotated object categories (classes), including the category ID and the category name.

#### Source

The training data was collected directly from the CADOT competition. The data collection and annotation process was carried out by [**please fill in information about the individuals/organization responsible for the annotation**].

#### Dataset Structure

The training split includes a collection of images related to [**please fill in the specific context of the CADOT competition, e.g., technical drawings, 3D model renders, CAD software interfaces, etc.**]. Each image may contain one or more objects belonging to the categories defined in the `categories` section of the COCO format.

* **Training Image Directory:** `[**please fill in the path or describe the location of the training image files**]`
* **Training Annotation File (JSON):** `[**please fill in the name and path (if applicable) of the JSON file containing the COCO format annotations for the training set**]` (This file will contain information about `images`, `annotations`, and `categories` for the training dataset).
