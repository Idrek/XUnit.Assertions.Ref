# Xunit assertions 

Commit: [c27a91f8cbcee37cb45699a3a81287bca225e876](https://github.com/xunit/xunit/tree/c27a91f8cbcee37cb45699a3a81287bca225e876)

## Summary

- [Boolean asserts](https://github.com/Idrek/XUnit.Assertions.Ref#boolean-asserts)
- [Collection asserts](https://github.com/Idrek/XUnit.Assertions.Ref#collection-asserts)
- [Equality asserts](https://github.com/Idrek/XUnit.Assertions.Ref#equality-asserts)
- [Equivalence asserts](https://github.com/Idrek/XUnit.Assertions.Ref#equivalence-asserts)
- [Event asserts](https://github.com/Idrek/XUnit.Assertions.Ref#event-asserts)
- [Exception asserts](https://github.com/Idrek/XUnit.Assertions.Ref#exception-asserts)
- [Fail asserts](https://github.com/Idrek/XUnit.Assertions.Ref#fail-asserts)
- [Identity asserts](https://github.com/Idrek/XUnit.Assertions.Ref#identity-asserts)
- [Multiple asserts](https://github.com/Idrek/XUnit.Assertions.Ref#multiple-asserts)
- [Null asserts](https://github.com/Idrek/XUnit.Assertions.Ref#null-asserts)
- [Property asserts](https://github.com/Idrek/XUnit.Assertions.Ref#property-asserts)
- [Range asserts](https://github.com/Idrek/XUnit.Assertions.Ref#range-asserts)
- [Set asserts](https://github.com/Idrek/XUnit.Assertions.Ref#set-asserts)
- [Skip asserts](https://github.com/Idrek/XUnit.Assertions.Ref#skip-asserts)
- [String/Span/Memory asserts](https://github.com/Idrek/XUnit.Assertions.Ref#stringspanmemory-asserts)
- [Regex asserts](https://github.com/Idrek/XUnit.Assertions.Ref#regex-asserts)
- [Type asserts](https://github.com/Idrek/XUnit.Assertions.Ref#type-asserts)

## Boolean asserts

```Assert.True(expression)``` 
  - [TrueTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/TrueTests.cs)
  - [BooleanAssertsTests/True](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/BooleanAssertsTests.cs#L58)

```Assert.False(expression)``` 
  - [FalseTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/FalseTests.cs)
  - [BooleanAssertsTests/False](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/BooleanAssertsTests.cs#L7)

## Collection asserts

`Assert.All<T>(collection, predicate)`

`Assert.All(collection, predicate)`

  - [CollectionAssertsTests/All](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L16)

`Assert.AllAsync<T>(collection, predicate)`

`Assert.AllAsync(collection, predicate)`

  - [CollectionAssertsTests/AllAsync](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L89)

`Assert.Collection(collection)`

`Assert.Collection(collection, predicate1, ..., predicateN)`

  - [CollectionAssertsTests/Collection](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L182)

`Assert.CollectionAsync(collection)`

`Assert.CollectionAsync(collection, predicate1, ..., predicateN)`

  - [CollectionAssertsTests/CollectionAsync](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L254)

`Assert.Contains(element, collection)`

`Assert.Contains(element, collection, comparer)`

`Assert.Contains(collection, predicate)`

`Assert.Contains<T>(collection, predicate)`

  - [CollectionAssertsTests/Contains](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L342)

  - [CollectionAssertsTests/Contains_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L477)

  - [CollectionAssertsTests/Contains_WithPredicate](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L521)

`Assert.Distinct(collection)`

`Assert.Distinct<T>(collection)`

`Assert.Distinct(collection, comparer)`

  - [CollectionAssertsTests/Distinct](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L547)

`Assert.DoesNotContain(element, collection)`

`Assert.DoesNotContain(element, collection, comparer)`

`Assert.DoesNotContain(collection, predicate)`

  - [CollectionAssertsTests/DoesNotContain](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L613)

  - [CollectionAssertsTests/DoesNotContain_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L765)

  - [CollectionAssertsTests/DoesNotContain_WithPredicate](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L802)

`Assert.Empty(collection)`

  - [CollectionAssertsTests/Empty](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L828)

`Assert.NotEmpty(collection)`

  - [CollectionAssertsTests/NotEmpty](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1083)

`Assert.Single(collection)`

`Assert.Single<T>(collection)`

`Assert.Single(collection, element)`

`Assert.Single(collection, predicate)`

`Assert.Single<T>(collection, predicate)`

  - [CollectionAssertsTests/Single_NonGeneric](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1170)

  - [CollectionAssertsTests/Single_NonGeneric_WithObject](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1222)

  - [CollectionAssertsTests/Single_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1269)

  - [CollectionAssertsTests/Single_Generic_WithPredicate](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1320)

## Equality asserts

`Assert.Equal(expected, actual)`

`Assert.Equal<T>(expected, actual)`

`Assert.Equal(expected, actual, comparer)`

`Assert.Equal(expected, actual, precision)`

`Assert.Equal(expected, actual, precision, MidpointRounding)`

`Assert.Equal(expected, actual, tolerance)`

  - [CollectionAssertsTests/Equal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L879)

  - [CollectionAssertsTests/Equal_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1057)

  - [EqualityAssertsTests/Equal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L11)

  - [EqualityAssertsTests/Equal_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L732)

  - [EqualityAssertsTests/Equal_Decimal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L763)

  - [EqualityAssertsTests/Equal_Double](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L780)

  - [EqualityAssertsTests/Equal_Double_MidPointRounding](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L810)

  - [EqualityAssertsTests/Equal_Double_Tolerance](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L833)

  - [EqualityAssertsTests/Equal_Float](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L900)

`Assert.StrictEqual(expected, actual)`

  - [EqualityAssertsTests/StrictEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L967)

`Assert.NotEqual(expected, actual)`

`Assert.NotEqual(expected, actual, comparer)`

`Assert.NotEqual(expected, actual, precision)`

  - [CollectionAssertsTests/NotEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1114)

  - [CollectionAssertsTests/NotEqual_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1135)

  - [EqualityAssertsTests/NotEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1001)

  - [EqualityAssertsTests/NotEqual_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1122)

  - [EqualityAssertsTests/NotEqual_Decimal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1146)

  - [EqualityAssertsTests/NotEqual_Double](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1168)

`Assert.NotStrictEqual(expected, actual)`

  - [EqualityAssertsTests/NotStrictEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1190)

## Equivalence asserts

`Assert.Equivalent(expected, actual)`

<code>Assert.Equivalent(expected, actual, strict: _boolean_)</code>

  - [EquivalenceAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EquivalenceAssertsTests.cs#L8)

## Event asserts

`Assert.Raises<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/Raises_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L8)

`Assert.RaisesAny<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/RaisesAny_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L59)

`Assert.RaisesAsync<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/RaisesAsync_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L162)

`Assert.RaisesAnyAsync<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/RaisesAnyAsync_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L109)

## Exception asserts

`Assert.Throws<E>(predicate)`

`Assert.ThrowsAsync<E>(predicate)`

`Assert.ThrowsAny<E>(predicate)`

`Assert.ThrowsAnyAsync<E>(predicate)`

`Assert.Throws(exceptionType, predicate)`

`Assert.ThrowsAsync(exceptionType, predicate)`

`Assert.Throws<E>(paramName, predicate)`

`Assert.ThrowsAsync<E>(paramName, predicate)`

  - [ExceptionAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/ExceptionAssertsTests.cs#L7)

## Fail asserts

`Assert.Fail(message)`

  - [FailAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/FailAssertsTests.cs#L5)

## Identity asserts

`Assert.Same(expected, actual)`

  - [SameTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/SameTests.cs)

  - [IdentityAssertsTests/Same](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/IdentityAssertsTests.cs#L26)  

`Assert.NotSame(expected, actual)`

  - [NotSameTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NotSameTests.cs)

  - [IdentityAssertsTests/NotSame](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/IdentityAssertsTests.cs#L6)

## Multiple asserts

`Assert.Multiple()`

`Assert.Multiple(predicate1, ..., predicateN)`

  - [MultipleAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/MultipleAssertsTests.cs)

## Null asserts

`Assert.Null(expression)`

  - [NullTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NullTests.cs)

  - [NullAssertsTests/Null](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/NullAssertsTests.cs#L25)

`Assert.NotNull(expression)`

  - [NotNullTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NotNullTests.cs)

  - [NullAssertsTests/NotNull](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/NullAssertsTests.cs#L7)

## Property asserts

`Assert.PropertyChanged(element, property, predicate)`

  - [PropertyChangedTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/PropertyChangedTests.cs)

  - [PropertyAssertsTests/PropertyChanged](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/PropertyAssertsTests.cs#L9)

`Assert.PropertyChangedAsync(element, property, predicate)`

  - [PropertyAssertsTests/PropertyChangedAsync](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/PropertyAssertsTests.cs#L80)

## Range asserts

`Assert.InRange(value, minRange, maxRange)`

`Assert.InRange(value, minRange, maxRange, comparer)`

  - [InRangeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/InRangeTests.cs)

  - [RangeAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/RangeAssertsTests.cs)

`Assert.NotInRange(value, minRange, maxRange)`

`Assert.NotInRange(value, minRange, maxRange, comparer)`

  - [NotInRangeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NotInRangeTests.cs)

  - [RangeAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/RangeAssertsTests.cs)

## Set asserts

`Assert.Subset(expected, actual)`

  - [SetAssertsTests/Subset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L8)

`Assert.ProperSubset(expected, actual)`

  - [SetAssertsTests/ProperSubset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L52)

`Assert.Superset(expected, actual)`

  - [SetAssertsTests/Superset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L96)

`Assert.ProperSuperset(expected, actual)`

  - [SetAssertsTests/ProperSuperset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L140)

## Skip asserts

`Assert.Skip(testExpression)`

`Assert.SkipUnless(boolExpression, testExpression)`

`Assert.SkipWhen(boolExpression, testExpression)`

  - [SkipAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SkipAssertsTests.cs)

## String/Span/Memory asserts

`Assert.StartsWith(search, text)`

`Assert.StartsWith(search, text, comparison)`

`Assert.EndsWith(search, text)`

`Assert.EndsWith(search, text, comparison)`

  - [MemoryAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/MemoryAssertsTests.cs)

  - [SpanAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SpanAssertsTests.cs)

  - [StringAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/StringAssertsTests.cs)

## Regex asserts

`Assert.Matches(match, text)`

`Assert.DoesNotMatch(match, text)`

  - [StringAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/StringAssertsTests.cs)

## Type asserts

`Assert.IsAssignableFrom(type, expression)`

`Assert.IsAssignableFrom<T>(expression)`

  - [IsAssignableFromTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/IsAssignableFromTests.cs)

`Assert.IsNotType(type, expression)`

`Assert.IsNotType<T>(expression)`

  - [IsNotTypeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/IsNotTypeTests.cs)

`Assert.IsType(type, expression)`

`Assert.IsType<T>(expression)`

  - [IsTypeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/IsTypeTests.cs)
