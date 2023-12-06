---
title: Toggle column
---
import AutoScreenshot from "@components/AutoScreenshot.astro"

## Overview

The toggle column allows you to render a toggle button inside the table, which can be used to update that database record without needing to open a new page or a modal:

```php
use Filament\Tables\Columns\ToggleColumn;

ToggleColumn::make('is_admin')
```

<AutoScreenshot name="tables/columns/toggle/simple" alt="Toggle column" version="3.x" />

## Lifecycle hooks

Hooks may be used to execute code at various points within the toggle's lifecycle:

```php
ToggleColumn::make()
    ->updateStateUsing(function ($record, $state) {
        // to update State
    })
```
