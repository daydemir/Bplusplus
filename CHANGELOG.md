# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.3] - 2025-07-30

### Added
- New `inference.py` module for streamlined model inference
- New `tracker.py` module for video object tracking functionality
- YOLOv11 weights support for improved object detection

### Changed
- Streamlined package architecture by moving modules from hierarchical structure to root level
- Updated model pipeline to support video inference with tracking
- Simplified prepare.py functionality
- Updated full_pipeline.ipynb notebook with new workflow

### Removed
- Removed resnet-specific test and train modules (`resnet/test.py`, `resnet/train.py`)
- Removed `train_validate.py` module
- Removed hierarchical directory structure

## [1.2.2] - 2024-12-19

### Added
- Enhanced GBIF occurrence filtering in `collect.py`:
  - Added `basisOfRecord` filter to include only HUMAN_OBSERVATION, LIVING_SPECIMEN, MACHINE_OBSERVATION, OBSERVATION, and OCCURRENCE records
  - Added `lifeStage` filter to include only Adult specimens
  - These changes improve the quality and relevance of collected images by filtering out juvenile specimens and unsuitable record types