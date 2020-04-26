# ION Memory Driver for CedarX on Mainline Linux v5.4
### Based on Google Android ION driver

Ovewrite on drivers/staging/android

dts
```
ion: ion {
    compatible = "allwinner,sunxi-ion";
    status = "disabled";
    heap_cma@0{
        compatible = "allwinner,cma";
        heap-name  = "cma";
        heap-id    = <0x4>;
        heap-base  = <0x0>;
        heap-size  = <0x0>;
        heap-type  = "ion_cma";
    };
};
```
