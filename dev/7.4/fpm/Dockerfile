FROM chialab/php:7.4-fpm
LABEL maintainer="dev@chialab.io"

# Install XDebug.
RUN pecl install xdebug \
    && echo "zend_extension=\"$(php-config --extension-dir)/xdebug.so\"" > $PHP_INI_DIR/conf.d/xdebug.ini
