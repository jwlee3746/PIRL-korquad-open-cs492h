# [Tean 13 PIRL] Empirical Studies for Answering KorQuAD-OPEN
Empirical Studies for Answering KorQuAD-OPEN

## Usage

### Submit oue SOTA model
nsml submit kaist_13/korquad-open-ldbd/135/PIRL_gs41000_e1

### Train SOTA model in NSML
```bash
sh run_nsml_base.sh
```

### Train ensemble model in NSML
```bash
sh run_nsml_ensemble.sh
```

### Train small model in NSML
```bash
sh run_nsml.sh
```

### Code Completed Part
```
open_squad_metrics_ver1.py : def normalize_answer(s)

run_squad_base.py : class ElectraForQuestionAnswering(ElectraPreTrainedModel)

run_squad_base_ensemble.py : class EnsembleElectraBertForQuestionAnswering(nn.Module)
                             class SelfEnsembleElectraForQuestionAnswering(nn.Module)
                             about model_2, config2
