# Working Commands

- ## Training from scratch:
```
python train.py -d /workspace/dataset/SemanticKITTI -ac config/arch/LENet.yaml -dc config/labels/semantic-kitti.yaml -l /workspace/traning_logs > train_lenet.txt 2>&1
``` 

- ## Command  to run inference:

```
python infer.py -d /workspace/dataset/SemanticKITTI -m /work/akmt/datset/lenet_trained/ -l /workspace/trained_models_predictions -s valid
```

- ## For  Model's Predictions Visualization for Sequence 08 (Valid):
 
 ```
python visualize.py -w kitti -d /work/akmt/dataset/SemanticKITTI -s 08 -p /work/akmt/LENet/trained_models_predictions
 ```

- ## Command to run inference on Slamantic: 

```
python infer_target.py -d /workspace/dataset/SLAMANTIC -m /workspacexperiment/lenet_trained -l /workspace/test_slamantic_predictions -s test 

```