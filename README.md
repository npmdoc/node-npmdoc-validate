# api documentation for  [validate (v3.0.1)](https://github.com/eivindfjeldstad/validate#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-validate.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-validate) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-validate.svg)](https://travis-ci.org/npmdoc/node-npmdoc-validate)
#### Validate object properties in javascript.

[![NPM](https://nodei.co/npm/validate.png?downloads=true)](https://www.npmjs.com/package/validate)

[![apidoc](https://npmdoc.github.io/node-npmdoc-validate/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-validate_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-validate/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-validate/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-validate/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Eivind Fjeldstad"
    },
    "bugs": {
        "url": "https://github.com/eivindfjeldstad/validate/issues"
    },
    "dependencies": {
        "component-type": "1.0.0",
        "eivindfjeldstad-dot": "0.0.1",
        "typecast": "0.0.1"
    },
    "description": "Validate object properties in javascript.",
    "devDependencies": {
        "mocha": "~1.14.0",
        "should": "~2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "798487b3a146ceb3c903ecd986c7e67db9478652",
        "tarball": "https://registry.npmjs.org/validate/-/validate-3.0.1.tgz"
    },
    "gitHead": "f4a79b3332fd7c439ad6f7c1846685589cfdaa10",
    "homepage": "https://github.com/eivindfjeldstad/validate#readme",
    "keywords": [
        "validation",
        "validate",
        "valid",
        "object"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "eivifj",
            "email": "eivind.fjeldstad@gmail.com"
        }
    ],
    "name": "validate",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/eivindfjeldstad/validate.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "3.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module validate](#apidoc.module.validate)
1.  [function <span class="apidocSignatureSpan">validate.</span>property (name, schema)](#apidoc.element.validate.property)
1.  object <span class="apidocSignatureSpan">validate.</span>property.prototype

#### [module validate.property](#apidoc.module.validate.property)
1.  [function <span class="apidocSignatureSpan">validate.</span>property (name, schema)](#apidoc.element.validate.property.property)

#### [module validate.property.prototype](#apidoc.module.validate.property.prototype)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>each (fn, msg)](#apidoc.element.validate.property.prototype.each)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>match (regexp, msg)](#apidoc.element.validate.property.prototype.match)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>message (msg)](#apidoc.element.validate.property.prototype.message)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>path (path, rules)](#apidoc.element.validate.property.prototype.path)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>required (bool, msg)](#apidoc.element.validate.property.prototype.required)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>type (name, msg)](#apidoc.element.validate.property.prototype.type)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>typecast (val)](#apidoc.element.validate.property.prototype.typecast)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>use (fn, msg)](#apidoc.element.validate.property.prototype.use)
1.  [function <span class="apidocSignatureSpan">validate.property.prototype.</span>validate (value, ctx)](#apidoc.element.validate.property.prototype.validate)



# <a name="apidoc.module.validate"></a>[module validate](#apidoc.module.validate)

#### <a name="apidoc.element.validate.property"></a>[function <span class="apidocSignatureSpan">validate.</span>property (name, schema)](#apidoc.element.validate.property)
- description and source-code
```javascript
function Property(name, schema) {
  this.fns = [];
  this.name = name;
  this.schema = schema;
  this._type = undefined;
  this.msg = 'validation failed for path ' + name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validate.property"></a>[module validate.property](#apidoc.module.validate.property)

#### <a name="apidoc.element.validate.property.property"></a>[function <span class="apidocSignatureSpan">validate.</span>property (name, schema)](#apidoc.element.validate.property.property)
- description and source-code
```javascript
function Property(name, schema) {
  this.fns = [];
  this.name = name;
  this.schema = schema;
  this._type = undefined;
  this.msg = 'validation failed for path ' + name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validate.property.prototype"></a>[module validate.property.prototype](#apidoc.module.validate.property.prototype)

#### <a name="apidoc.element.validate.property.prototype.each"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>each (fn, msg)](#apidoc.element.validate.property.prototype.each)
- description and source-code
```javascript
each = function (fn, msg) {
  return this.use(each(fn), msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.property.prototype.match"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>match (regexp, msg)](#apidoc.element.validate.property.prototype.match)
- description and source-code
```javascript
match = function (regexp, msg) {
  return this.use(match(regexp), msg);
}
```
- example usage
```shell
...

You can also add paths to a schema by using the chainable API
'''js
user
.path('username')
.type('string')
.required()
.match(/[a-z]{2,16}/)
.message('Username must be 2-16 chars.');

user
.path('address.zip')
.type('string')
.required()
.match(/[0-9]+/)
...
```

#### <a name="apidoc.element.validate.property.prototype.message"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>message (msg)](#apidoc.element.validate.property.prototype.message)
- description and source-code
```javascript
message = function (msg) {
  return this.msg = msg;
}
```
- example usage
```shell
...
You can also add paths to a schema by using the chainable API
'''js
user
.path('username')
.type('string')
.required()
.match(/[a-z]{2,16}/)
.message('Username must be 2-16 chars.');

user
.path('address.zip')
.type('string')
.required()
.match(/[0-9]+/)
.message('Zip is required.');
...
```

#### <a name="apidoc.element.validate.property.prototype.path"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>path (path, rules)](#apidoc.element.validate.property.prototype.path)
- description and source-code
```javascript
path = function (path, rules) {
  return this.schema(path, rules);
}
```
- example usage
```shell
...
errors[0].path //=> 'address.street'
errors[0].message //=> 'Street is required.'
'''

You can also add paths to a schema by using the chainable API
'''js
user
.path('username')
.type('string')
.required()
.match(/[a-z]{2,16}/)
.message('Username must be 2-16 chars.');

user
.path('address.zip')
...
```

#### <a name="apidoc.element.validate.property.prototype.required"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>required (bool, msg)](#apidoc.element.validate.property.prototype.required)
- description and source-code
```javascript
required = function (bool, msg) {
  if ('string' == typeof bool) msg = bool;
  return this.use(required(bool), msg);
}
```
- example usage
```shell
...
'''

You can also add paths to a schema by using the chainable API
'''js
user
.path('username')
.type('string')
.required()
.match(/[a-z]{2,16}/)
.message('Username must be 2-16 chars.');

user
.path('address.zip')
.type('string')
.required()
...
```

#### <a name="apidoc.element.validate.property.prototype.type"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>type (name, msg)](#apidoc.element.validate.property.prototype.type)
- description and source-code
```javascript
type = function (name, msg) {
  this._type = name;
  return this.use(type(name), msg);
}
```
- example usage
```shell
...
errors[0].message //=> 'Street is required.'
'''

You can also add paths to a schema by using the chainable API
'''js
user
.path('username')
.type('string')
.required()
.match(/[a-z]{2,16}/)
.message('Username must be 2-16 chars.');

user
.path('address.zip')
.type('string')
...
```

#### <a name="apidoc.element.validate.property.prototype.typecast"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>typecast (val)](#apidoc.element.validate.property.prototype.typecast)
- description and source-code
```javascript
typecast = function (val) {
  return typecast(val, this._type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.property.prototype.use"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>use (fn, msg)](#apidoc.element.validate.property.prototype.use)
- description and source-code
```javascript
use = function (fn, msg) {
  this.fns.push([fn, msg]);
  return this;
}
```
- example usage
```shell
...
 * @param {String} [msg]
 * @return {Property}
 * @api public
 */

required: function (bool, msg) {
  if ('string' == typeof bool) msg = bool;
  return this.use(required(bool), msg);
},

/**
 * Is of type 'name'
 *
 * @param {String} name
 * @param {String} [msg]
...
```

#### <a name="apidoc.element.validate.property.prototype.validate"></a>[function <span class="apidocSignatureSpan">validate.property.prototype.</span>validate (value, ctx)](#apidoc.element.validate.property.prototype.validate)
- description and source-code
```javascript
validate = function (value, ctx) {
  var fns = this.fns;

  for (var i = 0; i < fns.length; i++) {
    var fn = fns[i];
    var valid = fn[0].call(ctx, value);
    if (!valid) return error(this, fn[1]);
  }

  return false;
}
```
- example usage
```shell
...
      type: 'string',
      required: true,
      message: 'City is required.'
    }
  },
});

var errors = user.validate(obj);
'''

Each error has a '.path', describing the full path of the property that failed validation,
and a '.message' property.

'''js
errors[0].path //=> 'address.street'
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
