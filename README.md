# BERT_NLP_practice

*Install
bert-tensorflow

bert-for-tf2

sentencepiece

tensorflow_hub

tensorflow

tensorflow-addons



# TF2 upgrade -- anaconda3\envs\bert_nlp\Lib\site-packages\bert\

(1) modeling.py
'''
def layer_norm(input_tensor, name=None):
  return contrib_layers.layer_norm(
      inputs=input_tensor, begin_norm_axis=-1, begin_params_axis=-1, scope=name)
'''
 
def layer_norm(input_tensor, name=None):
  """Run layer normalization on the last dimension of the tensor."""
  layer_norma = tf.keras.layers.LayerNormalization(axis = -1)
  return layer_norma(input_tensor)
  
(2) run_classifier.py
    from bert import bert_tokenization
   comment [tokenization.printable_text(x) for x in tokens]))
   [bert_tokenization.printable_text(x) for x in tokens]))
