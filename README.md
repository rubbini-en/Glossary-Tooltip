# Glossary Tooltip Drupal Module

The Glossary Tooltip is a custom Drupal 8/9 module for automatically creating tooltips for terms defined in a glossary vocabulary.

[![Drupal 8/9](https://img.shields.io/badge/Drupal-8/9-blue.svg)](https://www.drupal.org)

## Table of Contents
1. [Features](#features)
2. [Requirements](#requirements)
3. [Installation](#installation)
4. [Configuration](#configuration)

## Features <a name="features"></a>

- **Term Highlighting**: Scans the content of your nodes for terms defined in the 'glossary' vocabulary.
- **Automatic Tooltip**: Wraps found terms in a span with a tooltip containing the term's description.
- **Cache Optimization**: Utilizes Drupal's caching system to enhance performance.
- **Content Type Agnostic**: Can be used with any content type.

## Requirements <a name="requirements"></a>

- Drupal 8/9
- A vocabulary named 'glossary' with terms defined

## Installation <a name="installation"></a>

1. Copy the `glossary_tooltip` directory to your Drupal `modules/custom` directory.
2. Navigate to the `Extend` page on your Drupal site (`/admin/modules`).
3. Find 'Glossary Tooltip' in the module list, check the box next to it, then click `Install`.

## Configuration <a name="configuration"></a>

Once installed, you need to create a vocabulary named 'glossary'. The terms added to this vocabulary will be used for tooltip creation; the term name is used for matching in the content, and the description becomes the tooltip text.

After configuration, the module will automatically parse any new or updated nodes for glossary terms and apply the tooltips as needed.
