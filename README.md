# PM 2.5 Air Quality sensor for espidf

This library is an adatation of [Adafruit PM2.5 Air Quality sensor](https://github.com/adafruit/Adafruit_PM25AQI) library  for espidf

This library for espidf works with [PM2.5 Air Quality Module](https://shop.m5stack.com/products/pm2-5-air-quality-kit) from M5stack.

## How to Add to you project
### Using platformio

- Add `https://github.com/bjay-wk/pm25-espidf.git` to the `lib_deps`in `platformio.ini`.

### Using Espidf
In `src/idf_component.yml` of your project add

```yaml
pm25-espidf:
  git: https://github.com/bjay-wk/pm25-espidf.git
```

And in `src/CMakeLists.txt` of your project

```make
idf_component_register(...
    REQUIRES pm25-espidf
    ...
)
```
