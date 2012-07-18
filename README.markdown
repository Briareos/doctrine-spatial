# Doctrine Spatial Extension

## Installation

Doctrine\Spatial can be installed using the [Composer](http://packagist.org/) tool. You can either add `doctrine/spatial` to your package dependencies, or if you want to install Doctrine\Spatial as standalone, go to the main directory of this package and run:

    $ wget http://getcomposer.org/composer.phar
    $ php composer.phar install
    
## Integration with Symfony2

Update your `config.yml` file and under `doctrine.dbal` add the following types:

    doctrine:
        dbal:
            types:
                point:              Doctrine\Spatial\DBAL\Types\PointType
                linestring:         Doctrine\Spatial\DBAL\Types\LineStringType
                polygon:            Doctrine\Spatial\DBAL\Types\PolygonType
                multipoint:         Doctrine\Spatial\DBAL\Types\MultiPointType
                multilinestring:    Doctrine\Spatial\DBAL\Types\MultiLineStringType
                multipolygon:       Doctrine\Spatial\DBAL\Types\MultiPolygonType
                geometrycollection: Doctrine\Spatial\DBAL\Types\GeometryCollectionType


## License

The Doctrine Spatial Extension is released under the [MIT License](https://github.com/Briareos/doctrine-spatial/blob/master/LICENSE).
