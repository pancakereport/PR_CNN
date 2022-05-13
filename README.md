# Silas Gifford Honors Thesis

Here is the code, images, and data on the populations of interest in Point Reyes National Seashore.

## Basic Info

1. Harbor Seals
   * Date Range:
     * Pupping Season: March to May
       * Age classes: "adult" and "pup"
     * Molting Season: June and July
       * Age class: "adult"
   * Drakes Estero
   * Double Point
   * Tomales Bay
   * Tomales Point
   * Point Reyes
2. Elephant Seals
   * Date Range:
     * Pupping Season: November to March with peak between 1/26 and 2/2
       * Age classes: "bull" (adult male), "cow" (adult female), and "pup" (baby)
   * Point Reyes Headlands
   * Drakes Beach
   * South Beach


## Recreate my work by...
* Using the full images pulled from Google Earth found under `Images`
* Tile these images with  `Cold/Tile_Harbor_Seals.ipynb` and `Code/Tile_Elephant_Seals.ipynb`
* Create your own annotations via https://www.robots.ox.ac.uk/~vgg/software/via/app/via_image_annotator.html or use mine found in `Data/Harbor_Seal_Anno_csv.csv` and `Data/Elephant_Seal_Anno_csv`
* If you're using your own annotations, use this repo https://github.com/martinzlocha/anchor-optimization/ to get anchor configurations, or use mine at `Data/habor_config.ini` and `Data/elephant_config.ini`
* Convert annotations into the right format for Retinanet using `Code/Harbor_Seal_Annotations_Right_Format.ipynb` and `Code/Elephant_Seal_Annotations_Right_Format.ipynb` 
  * Please note that this code will give you randomized training, validation, and testing sets. If you want to train/test on specific imagery, you must change the code.
* Make sure you have Retinanet installed: https://github.com/fizyr/keras-retinanet
* To train on all harbor seal tiles, use `Code/Harbor_Seals_Run_Model_Full.ipynb`
* To train on harbor seal beach-only tiles, use `Code/Harbor_Seals_Run_Model_Beach.ipynb`
* To train on elephant seal beach-only tiles, use `Code/Elephant_Seals_Run_Model.ipynb`
* Use `Code/harbor_seal_visual_check.ipynb` and `Code/harbor_seal_visual_check.ipynb` to visualize model output or view model output in `Data/model_output`
