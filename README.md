fruit.zip 为数据集

目录：
	images：存放待检测的图片
	output：存放检测好的图片
	yolov3_mobilenet_v3_large_voc：存放模型，模型是使用paddleDetection训练好的


使用方法：
	1、安装paddle2.0.0以上版本
	2、安装库：pip install -r requirements.txt
	3、将yolov3_mobilenet_v3_large_voc.zip解压，yolov3_mobilenet_v3_large_voc文件夹下有4个文件infer_cfg.yml,model.pdiparams,model.pdiparams.info,model.pdmodel
	4、在目录下打开cmd，输入：python .\infer.py --model_dir=yolov3_mobilenet_v3_large_voc --image_file=images\mixed_6.jpg
	检测结果在output目录中