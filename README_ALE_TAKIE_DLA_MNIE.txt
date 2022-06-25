######### basics #########
modele do experiments/pre_trained_models
zdjecia do inputs
output wychodzi w results

######### odpalasz: #########
# wzor
python inference_realesrgan.py -n NAZWA_MODELU_BEZ_ROZSZERZENIA -i inputs (--face_enhance) OPCJONALNIE DO TWARZY
# przykład
python inference_realesrgan.py -n RealESRGAN_x4plus -i inputs --face_enhance

######### do kopiowania #########

# standard model
python inference_realesrgan.py -n RealESRGAN_x4plus -i inputs

# forest textures
python inference_realesrgan.py -n 4x_forest_textures_160k -i inputs

# skyrim textures
python inference_realesrgan.py -n 4x-SkyrimTexV2.1 -i inputs

# source engine textures
python inference_realesrgan.py -n 1x_DXTless_SourceEngine_170000_G -i inputs

# removing the damages done by dithering
python inference_realesrgan.py -n 1x_DitherDeleterV3-Smooth-[32]_115000_G -i inputs

#remove noise
python inference_realesrgan.py -n 1x_NoiseToner-Uniform-Detailed_100000_G -i inputs