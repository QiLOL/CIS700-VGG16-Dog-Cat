# CIS700-VGG16-Dog-Cat

## Running Instruction
1. `kaggle.json` is the key during download the dataset from Kaggle

2. `pretest_part1_pretrained_model.ipynb` will generate the pretrained model with original dataset, we can change the `update_params_name` to change the layer can be updated during the training

3. `pretest_part2_adversarial_example_dataset.ipynb` will generate the adversarial examples based on different $\epsilon$, change `t_eps` for different $\epsilon$ value.

4. `test1_continue_training.ipynb` do continuous training on adversarial dataset

5. `test2_continue_training_flipped_test3.ipynb` do continuous training on adversarial dataset but flipped label, for example, if one sample's label is Dog, it should be Dog in adversarial dataset, but in this step it will flip to Cat.

## The file in Google Drive
`model_ori_trained.pkl` the pretrained model1(Model1 in report)

`model_ori_trained2.pkl` Model2 in report

Model1 adversarial datasets:
`adv_samples_eps_0.007_pure.pkl`
`adv_samples_eps_0.0001_pure.pkl`
`adv_samples_eps_1e-05_pure.pkl`

Model2 adversarial datasets:
`adv_samples2_eps_0.01_pure.pkl`
`adv_samples2_eps_0.007_pure.pkl`
`adv_samples2_eps_0.0001_pure.pkl`
`adv_samples2_eps_1e-05_pure.pkl`


Continuous training with adversarial datasets on Model1:
`model_adv_trained1_0.007.pkl` `model_adv_trained1_0.0001.pkl` `model_adv_trained1_1e-05.pkl`

Continuous training with adversarial datasets on Model2:
`model_adv_trained2_0.01.pkl`
`model_adv_trained2_0.007.pkl` `model_adv_trained2_0.0001.pkl` `model_adv_trained2_1e-05.pkl`

Continuous training with adversarial datasets on Model1 but flipping label during training:
`model_adv_trained_flipped_0.007.pkl` `model_adv_trained_flipped_0.0001.pkl` `model_adv_trained_flipped_1e-05.pkl`

Continuous training with adversarial datasets on Model1 but flipping label during training:
`model_adv_trained2_flipped_0.01.pkl`
`model_adv_trained2_flipped_0.007.pkl` `model_adv_trained2_flipped_0.0001.pkl` `model_adv_trained2_flipped_1e-05.pkl`

The new model generated during test3:
`model_adv_new_net.pkl`