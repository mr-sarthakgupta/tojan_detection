# Code for NeurIPS Trojan Detection Competition

This repository contains code for the experiments and runs done while participating in the NeurIPS Trojan Detection Challenge. We primarily use two approaches: an updated version of MNTD and an approach based on Zest of Lime.

- Updated MNTD: This approach simply scaled and fine-tuned the base MNTD approach provided by the authors to create inputs whose corresponding outputs when processed could help predict whether a given model ia trojaned or benign.

- Updated Zest of Lime: Refactored the Zest of Lime code for quick compute on GPUs and used it as a metric to try and find the distance between trojaned and benign models. This approach is based off of the intuition that trojaned models should have a signicantly altered decision boundary at specific points when compared to a benign model trained for the same task.
