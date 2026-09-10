# Comparison of Existing Techniques #

This research focuses on two privacy-preserving techniques, which are k-Anonymity and Differential Privacy.

## k-Anonymity

k-Anonymity is a technique used to protect personal information by making some records look similar based on selected attributes. It can reduce the chance of identifying a person from the dataset.

One advantage of k-anonymity is that it is quite simple to understand and apply. However, it may still have some re-identification risk. When more generalization is applied, some useful information in the dataset may also be lost.

Other methods such as Mondrian k-anonymity and l-diversity have also been studied to improve the limitations of basic k-anonymity. In this research, only standard k-anonymity is used.

## Differential Privacy

Differential Privacy protects sensitive information by adding noise to the data or the results. The amount of noise is controlled using a privacy budget, which is represented by `ε`.

One advantage of Differential Privacy is that it provides a formal privacy guarantee. However, too much noise can affect the accuracy and usefulness of the data.

Some previous studies also use different versions of Differential Privacy to improve the balance between privacy and data utility. In this research, standard Differential Privacy is used with Laplace noise and `ε = 1.0`.

## Comparison

| Technique | How It Works | Strength | Limitation |
|---|---|---|---|
| k-Anonymity | Uses generalization and suppression | Simple and practical | Re-identification risk can still remain |
| Differential Privacy | Adds controlled noise | Strong privacy protection | Noise can reduce accuracy |

Both techniques aim to protect sensitive information, but they use different approaches. k-Anonymity changes the records to make them less identifiable, while Differential Privacy adds noise to the data.

In this research, both techniques are applied to the same UCI Adult Census Income dataset so that their results can be compared using the same evaluation criteria.
