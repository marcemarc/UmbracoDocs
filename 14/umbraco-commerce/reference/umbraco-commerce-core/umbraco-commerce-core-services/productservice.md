---
title: ProductService
description: API reference for ProductService in Umbraco Commerce
---
## ProductService

```csharp
public class ProductService : ServiceBase<ProductService>, IProductService
```

**Inheritance**

* Class [ServiceBase&lt;TSelf&gt;](servicebase-1.md)
* interface [IProductService](iproductservice.md)

**Namespace**
* [Umbraco.Commerce.Core.Services](README.md)

### Constructors

#### ProductService

```csharp
public ProductService(IRepositoryFactory repositoryFactory, IUnitOfWorkProvider uowProvider, 
    ILogger<ProductService> logger, ICacheAccessor cacheAccessor, IProductAdapter productAdapter, 
    IStockService stockService)
```


### Methods

#### GetProduct (1 of 2)

```csharp
public IProductSnapshot GetProduct(Guid storeId, string productReference, string languageIsoCode)
```

---

#### GetProduct (2 of 2)

```csharp
public IProductSnapshot GetProduct(Guid storeId, string productReference, 
    string productVariantRefernce, string languageIsoCode)
```


---

#### GetProductStock (1 of 2)

```csharp
public decimal? GetProductStock(Guid storeId, string productReference)
```

---

#### GetProductStock (2 of 2)

```csharp
public decimal? GetProductStock(Guid storeId, string productReference, 
    string productVariantReference)
```


---

#### GetProductVariantAttributes

```csharp
public IEnumerable<Attribute> GetProductVariantAttributes(Guid storeId, string productReference, 
    string languageIsoCode)
```


---

#### IncreaseProductStock (1 of 2)

```csharp
public void IncreaseProductStock(Guid storeId, string productReference, decimal increaseBy)
```

---

#### IncreaseProductStock (2 of 2)

```csharp
public void IncreaseProductStock(Guid storeId, string productReference, 
    string productVariantReference, decimal increaseBy)
```


---

#### ReduceProductStock (1 of 2)

```csharp
public void ReduceProductStock(Guid storeId, string productReference, decimal reduceBy)
```

---

#### ReduceProductStock (2 of 2)

```csharp
public void ReduceProductStock(Guid storeId, string productReference, 
    string productVariantReference, decimal reduceBy)
```


---

#### SearchProductSummaries

```csharp
public PagedResult<IProductSummary> SearchProductSummaries(Guid storeId, string languageIsoCode, 
    string term, long currentPage = 1, long itemsPerPage = 50)
```


---

#### SearchProductVariantSummaries

```csharp
public PagedResult<IProductVariantSummary> SearchProductVariantSummaries(Guid storeId, 
    string productReference, string languageIsoCode, string searchTerm, 
    IDictionary<string, IEnumerable<string>> attributes, long currentPage = 1, 
    long itemsPerPage = 50)
```


---

#### SetProductStock (1 of 2)

```csharp
public void SetProductStock(Guid storeId, string productReference, decimal value)
```

---

#### SetProductStock (2 of 2)

```csharp
public void SetProductStock(Guid storeId, string productReference, string productVariantReference, 
    decimal value)
```


---

#### TryGetProductStock (1 of 2)

```csharp
public bool TryGetProductStock(Guid storeId, string productReference, out decimal? stock)
```

---

#### TryGetProductStock (2 of 2)

```csharp
public bool TryGetProductStock(Guid storeId, string productReference, 
    string productVariantReference, out decimal? stock)
```


---

#### TryIncreaseProductStock (1 of 2)

```csharp
public bool TryIncreaseProductStock(Guid storeId, string productReference, decimal increaseBy)
```

---

#### TryIncreaseProductStock (2 of 2)

```csharp
public bool TryIncreaseProductStock(Guid storeId, string productReference, 
    string productVariantReference, decimal increaseBy)
```


---

#### TryReduceProductStock (1 of 2)

```csharp
public bool TryReduceProductStock(Guid storeId, string productReference, decimal reduceBy)
```

---

#### TryReduceProductStock (2 of 2)

```csharp
public bool TryReduceProductStock(Guid storeId, string productReference, 
    string productVariantReference, decimal reduceBy)
```


---

#### TrySetProductStock (1 of 2)

```csharp
public bool TrySetProductStock(Guid storeId, string productReference, decimal value)
```

---

#### TrySetProductStock (2 of 2)

```csharp
public bool TrySetProductStock(Guid storeId, string productReference, 
    string productVariantReference, decimal value)
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Core.dll -->