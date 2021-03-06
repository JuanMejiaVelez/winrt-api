---
-api-id: P:Windows.Storage.Search.QueryOptions.ApplicationSearchFilter
-api-type: winrt property
---

<!-- Property syntax
public string ApplicationSearchFilter { get;  set; }
-->

# Windows.Storage.Search.QueryOptions.ApplicationSearchFilter

## -description
Gets or sets an application-defined Advanced Query Syntax (AQS) string for filtering files by keywords or properties. This property is combined with the [UserSearchFilter](queryoptions_usersearchfilter.md) to create the query's search filter.

## -property-value
A simple keyword, or a string that conforms to Advanced Query Syntax (AQS). For more information, see [Using Advanced Query Syntax Programmatically](http://msdn.microsoft.com/library/76e33903-d063-48c0-9afe-912c3daa8237).

## -remarks
The application search filter should always use locale-invariant Advanced Query Syntax (AQS) syntax (such as [System.FileName](https://msdn.microsoft.com/library/windows/desktop/bb760703.aspx) instead of "filename" (because the term "filename" that is associated with the property [System.FileName](https://msdn.microsoft.com/library/windows/desktop/bb760703.aspx) is localized differently in different languages). This will ensure that the query returns the expected results on systems with non-English locales. Windows builds the search query by combining this property with the [UserSearchFilter](queryoptions_usersearchfilter.md) property.

## -examples

## -see-also
