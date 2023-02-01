# bUnwarpJ_code
This ImageJ/Fiji plugin performs 2D image registration based on elastic deformations represented by B-splines. The invertibility of the deformations is enforced through a consistency restriction.

## Running ImageJ/Fiji with Multiple parameters
- Command on Linux:
``./ImageJ-linux64 --ij2 --headless --run "hello.py" "name1='Mr',name2='Mrs Kraken'"``

## Running bUnwarpJ_code in headless mode through Linux Terminal
``/path/to/ImageJ-linux64 --ij2 --headless --run "/path/to/groovyscript/bUnwarpJ_Ana.groovy" "inputFilesDir='/path/to/inputFiles/images',beadsFile='/path/to/beadsFile/Sylvia Gutierrez-Erlandsson - Beads ref.lif - Image001.tif',outputDir='/path/to/outputFolder/results',fixedCh=0,headless=true"``
## Running bUnwarpJ_code in headless mode (my parameters) through Linux Terminal
``/home/anaacayuela/Desktop/fiji-linux64/Fiji.app/ImageJ-linux64 --ij2 --headless --run "/home/anaacayuela/Ana_pruebas_imageJ/bUnwarpJ/groovy/src/main/bUnwarpJ_Ana.groovy" "inputFilesDir='/home/anaacayuela/Ana_pruebas_imageJ/bUnwarpJ/paper/set_2/images',beadsFile='/home/anaacayuela/Ana_pruebas_imageJ/bUnwarpJ/paper/set_2/ref_beads/Sylvia Gutierrez-Erlandsson - Beads ref.lif - Image001.tif',outputDir='/home/anaacayuela/Ana_pruebas_imageJ/bUnwarpJ/paper/set_2/results',fixedCh=0,headless=true"``

### Optionally Avanced Parameters for elastic registration can be set as arguments:
- #@Integer(label="Registration Mode", value=1) mode
- #@Integer(label="Image Subsample Factor", value=0) img_subsamp_fact
- #@Integer(label="Initial Deformation", value=0) min_scale_deformation
- #@Integer(label="Final Deformation", value=2) max_scale_deformation
- #@Double(label="Divergence Weight", value=0.0) divWeight
- #@Double(label="Curl Weight", value=0.0) curlWeight
- #@Double(label="Landmark Weight", value=0.0) landmarkWeight
- #@Double(label="Image Weight", value=1.0) imageWeight
- #@Double(label="Consistency Weight", value=10.0) consistencyWeight
- #@Double(label="Stop Threshold", value=0.01) stopThreshold
