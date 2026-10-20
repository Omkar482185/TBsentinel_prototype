# TBSentinel

### Federated Multimodal AI for Early Tuberculosis Detection and Assessment

TBSentinel is a research-oriented project exploring the use of multimodal artificial intelligence and federated learning for tuberculosis detection and the assessment of lung-related diseases.

The proposed system combines chest X-ray images, clinical notes, and structured clinical or laboratory data to investigate how multiple data modalities can support machine-learning research while exploring privacy-preserving collaborative training.

**Current status:** Initial Figma UI/UX prototype and project documentation. The AI models, multimodal pipeline, and federated learning implementation are planned unless explicitly marked as completed below.

## Project Objectives

- Explore multimodal learning using chest X-rays, clinical notes, and structured clinical data.
- Investigate federated learning across simulated hospital nodes without sharing raw training data between nodes.
- Explore differential privacy and secure communication for privacy-aware collaborative training.
- Investigate model explainability using Grad-CAM and SHAP.
- Evaluate model performance, robustness, and limitations using appropriate datasets and evaluation metrics.

## UI/UX Prototype

The initial interface was designed in Figma to establish the proposed user experience and workflows.

**Figma prototype:** [[Open the TBSentinel design](https://www.figma.com/proto/6XBeY936Mw49Q3QZ9l5iB7/TBSentinel-Prototype?node-id=1005-259&t=dgQWYqgVWR68a4T6-1)]


## Proposed System Architecture

1. **Data inputs:** Chest X-ray images, clinical notes, and structured clinical or laboratory data.
2. **Preprocessing:** Prepare and validate each modality for model training and evaluation.
3. **Local model training:** Train models on data held by individual simulated clients.
4. **Federated aggregation:** Combine model updates without centralizing raw training data.
5. **Multimodal assessment:** Explore combining information from multiple modalities.
6. **Explainability and evaluation:** Investigate model explanations and evaluate performance on appropriate test datasets.

This architecture is a proposed workflow, not a claim that the complete system is operational.

## Planned Technology Stack

| Component | Technologies under consideration |
|---|---|
| Programming language | Python |
| Deep learning | PyTorch |
| Image models | DenseNet121, EfficientNetV2, Vision Transformers |
| Federated learning | Flower or NVIDIA FLARE |
| Explainable AI | Grad-CAM, SHAP |
| Data modalities | Medical images, clinical text, structured data |

The final technology choices will depend on implementation requirements and experimental results.

## Development Roadmap

- [x] Initial UI/UX prototype in Figma
- [ ] Document system requirements and architecture
- [ ] Prepare suitable datasets and preprocessing pipelines
- [ ] Develop and evaluate baseline image models
- [ ] Explore multimodal data integration
- [ ] Implement federated learning simulation
- [ ] Investigate privacy-preserving techniques
- [ ] Add explainability and evaluation reports
- [ ] Document limitations and validation requirements

## Repository Structure

```text
TBSentinel/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   └── screenshots/
└── prototype/
    └── figma-link.md
```

## Responsible Use

TBSentinel is intended for educational and research purposes. It is not a clinically validated diagnostic system and must not be used as a substitute for professional medical assessment.

Any future model predictions will require appropriate evaluation and validation. Do not upload identifiable patient information, confidential clinical records, API keys, or other sensitive data to this repository.

## Contributing

Contributions to documentation, UI/UX, data preprocessing, model evaluation, federated learning, and explainable AI are welcome.

For substantial changes, open a GitHub Issue to discuss the proposed contribution before submitting a pull request. Please document implementation status and evaluation results accurately.

## License

Code that is owned by the project author and covered by this repository's license is distributed under the MIT License. See [LICENSE](LICENSE) for details.

Third-party assets, datasets, fonts, and other materials may have separate license terms. The Figma design is not automatically covered by the code license; refer to the design's separately stated permissions.
