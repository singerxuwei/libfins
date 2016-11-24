# Finslib API Reference

## Functions

### `finslib_monotonic_sec_timer( void );`

#### Parameters

| Parameter | Type | Description |
| :--- | :--- | :--- |

#### Returns

| Type | Description |
| :--- | :--- |
|`time_t`|A monotonic counter of the number of seconds which have passed since an unspecified starting point in time|

#### Description

The function `finslib_monotonic_sec_timer()` provides a seconds timer which is guaranteerd to be monotonic. This timer
is therefore not directly bound to the internal wall clock. Due to this it is immune for changes in the clock settings
and for changes in the time which happen during the transistion to and from daylight saving time.

The return value is the amount of seconds since an unspecified moment.