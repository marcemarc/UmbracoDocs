---
title: IDiscountRuleProvider
description: API reference for IDiscountRuleProvider in Umbraco Commerce
---
## IDiscountRuleProvider

```csharp
public interface IDiscountRuleProvider
```

**Namespace**
* [Umbraco.Commerce.Core.Discounts.Rules](README.md)

### Properties

#### Alias

```csharp
public string Alias { get; }
```


---

#### Description

```csharp
public string Description { get; }
```


---

#### Icon

```csharp
public string Icon { get; }
```


---

#### LabelView

```csharp
public string LabelView { get; }
```


---

#### Name

```csharp
public string Name { get; }
```


---

#### SettingDefinitions

```csharp
public IEnumerable<DiscountRuleProviderSettingDefinition> SettingDefinitions { get; }
```


### Methods

#### ValidateRule

```csharp
public DiscountRuleResult ValidateRule(DiscountRuleContext context, 
    IReadOnlyDictionary<string, string> settings)
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Core.dll -->