<html>
<center>
</h4>
<font color='blod' size="+2">Task Description!</font></h4>
</center>
<div class="markdown-google-sans">


</div>
<p>In this Notebook, we will fine-tune the models BERT and BioBERT for the NER test on NCBI disease corpora.
<!-- TODO(b/319266067) remove temporary advert after a few weeks. -->
<div class="markdown-google-sans">
  <h2>Biomedical corpora : </h2>
  <ul>
  <li><a href="https://huggingface.co/datasets/ncbi_disease#dataset-card-for-ncbi-disease">NCBI Disease</a></li>
  <p>This dataset contains the disease name and concept annotations of the NCBI disease corpus, a collection of 793 PubMed abstracts fully annotated at the mention and concept level to serve as a research resource for the biomedical natural language processing community.</p>
  <div>
  <center>
  <table border="1">
  <tr>
    <th>Dataset</th>
    <th>Train</th>
    <th>Validation</th>
    <th>Test</th>
  </tr>
  <tr>
    <td>Instances</td>
    <td>5433</td>
    <td>924</td>
    <td>941</td>
  </tr>
</table>
</h4>
<font color='blod' size="+2">Resultats</font></h4>
</center>
    model =bert-base-cased,biobert-v1.1
batch_size=16
 learning_rate=2e-5
optim=adamw_torch
num_train_epochs=8
eval_dataset= données de validation
    <table border="1">
  <tr>
    <th>Modèle</th>
    <th>Precision</th>
    <th>Recall</th>
    <th>F1</th>
  </tr>
  <tr>
    <td>BERT</td>
    <td>0.822678</td>
    <td>0.866582</td>
    <td>0.844059</td>
  </tr>
  <tr>
    <td>BioBERT</td>
    <td>0.830529</td>
    <td>0.878018</td>
    <td>0.853613</td>
  </tr>
</table>

</html>
