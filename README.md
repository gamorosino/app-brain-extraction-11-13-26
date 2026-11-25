# brain-extraction-13-11-26

<!-- brainlife-app:begin (generated from the App manifest; edit the manifest, not this block) -->

> **Skull-strips a T1-weighted image with FSL BET (optional robust centre estimation and bias/neck cleanup); appears to be an incomplete test copy of the Brain Extraction (FSL BET) App.**

Contains run_bet.sh and brain_extract.py but no main script, so it cannot run on brainlife as registered; run_bet.sh also writes to t1_brain/ rather than the registered t1w_brain output. Use the Brain Extraction (FSL BET) App instead.

| | |
|---|---|
| 📥 **Inputs** | `neuro/anat/t1w` |
| 📤 **Outputs** | `neuro/anat/t1w` |
| 🔗 **Run it** | [doi.org/10.25663/brainlife.app.998](https://doi.org/10.25663/brainlife.app.998) |

#### 📥 Inputs

| Input | Datatype | Required | Description |
|---|---|---|---|
| `t1w` | `neuro/anat/t1w` | yes | T1-weighted anatomical image to skull-strip. |

#### 📤 Outputs

| Output | Datatype | Description |
|---|---|---|
| `t1w_brain` | `neuro/anat/t1w` | Brain-extracted T1w image produced by FSL BET. |

<details>
<summary><b>⚙️ Parameters</b> (3)</summary>

| Parameter | Type | Default | Description |
|---|---|---|---|
| `frac` | number | `0.5` | Fractional intensity threshold (0–1). Smaller values give larger brain outlines. |
| `robust` | boolean | `false` | Run robust brain centre estimation, iterating BET several times. |
| `bias_neck_cleanup` | boolean | `false` | Run bias field correction and neck cleanup (-B flag). |

</details>

<!-- brainlife-app:end -->

