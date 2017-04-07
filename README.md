# api documentation for  [uglifyjs (v2.4.10)](http://lisperator.net/uglifyjs)  [![npm package](https://img.shields.io/npm/v/npmdoc-uglifyjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-uglifyjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-uglifyjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-uglifyjs)
#### JavaScript parser, mangler/compressor and beautifier toolkit

[![NPM](https://nodei.co/npm/uglifyjs.png?downloads=true)](https://www.npmjs.com/package/uglifyjs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-uglifyjs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "uglifyjs": "bin/uglifyjs"
    },
    "browserify": {
        "transform": [
            "uglify-to-browserify"
        ]
    },
    "bugs": {
        "url": "https://github.com/mishoo/UglifyJS2/issues"
    },
    "dependencies": {
        "async": "~0.2.6",
        "source-map": "0.1.34",
        "uglify-to-browserify": "~1.0.0",
        "yargs": "~1.3.3"
    },
    "description": "JavaScript parser, mangler/compressor and beautifier toolkit",
    "devDependencies": {
        "acorn": "~0.6.0",
        "escodegen": "~1.3.3",
        "esfuzz": "~0.3.1",
        "estraverse": "~1.5.1"
    },
    "directories": {},
    "dist": {
        "shasum": "632927319fa6a3da3fc91f9773ac27bfe6c3ee92",
        "tarball": "https://registry.npmjs.org/uglifyjs/-/uglifyjs-2.4.10.tgz"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "gitHead": "9de7199b88edb37753a36a9688d34a4be801f41b",
    "homepage": "http://lisperator.net/uglifyjs",
    "license": "BSD",
    "main": "tools/node.js",
    "maintainers": [
        {
            "name": "mytry",
            "email": "mytry@126.com"
        }
    ],
    "name": "uglifyjs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mishoo/UglifyJS2.git"
    },
    "scripts": {
        "test": "node test/run-tests.js"
    },
    "version": "2.4.10"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module uglifyjs](#apidoc.module.uglifyjs)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>ASSIGNMENT (str )](#apidoc.element.uglifyjs.ASSIGNMENT)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Accessor (props)](#apidoc.element.uglifyjs.AST_Accessor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Array (props)](#apidoc.element.uglifyjs.AST_Array)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Assign (props)](#apidoc.element.uglifyjs.AST_Assign)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Atom (props)](#apidoc.element.uglifyjs.AST_Atom)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Binary (props)](#apidoc.element.uglifyjs.AST_Binary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Block (props)](#apidoc.element.uglifyjs.AST_Block)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_BlockStatement (props)](#apidoc.element.uglifyjs.AST_BlockStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Boolean (props)](#apidoc.element.uglifyjs.AST_Boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Break (props)](#apidoc.element.uglifyjs.AST_Break)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Call (props)](#apidoc.element.uglifyjs.AST_Call)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Case (props)](#apidoc.element.uglifyjs.AST_Case)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Catch (props)](#apidoc.element.uglifyjs.AST_Catch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Conditional (props)](#apidoc.element.uglifyjs.AST_Conditional)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Const (props)](#apidoc.element.uglifyjs.AST_Const)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Constant (props)](#apidoc.element.uglifyjs.AST_Constant)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Continue (props)](#apidoc.element.uglifyjs.AST_Continue)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_DWLoop (props)](#apidoc.element.uglifyjs.AST_DWLoop)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Debugger (props)](#apidoc.element.uglifyjs.AST_Debugger)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Default (props)](#apidoc.element.uglifyjs.AST_Default)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Definitions (props)](#apidoc.element.uglifyjs.AST_Definitions)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Defun (props)](#apidoc.element.uglifyjs.AST_Defun)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Directive (props)](#apidoc.element.uglifyjs.AST_Directive)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Do (props)](#apidoc.element.uglifyjs.AST_Do)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Dot (props)](#apidoc.element.uglifyjs.AST_Dot)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_EmptyStatement (props)](#apidoc.element.uglifyjs.AST_EmptyStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Exit (props)](#apidoc.element.uglifyjs.AST_Exit)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_False (props)](#apidoc.element.uglifyjs.AST_False)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Finally (props)](#apidoc.element.uglifyjs.AST_Finally)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_For (props)](#apidoc.element.uglifyjs.AST_For)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ForIn (props)](#apidoc.element.uglifyjs.AST_ForIn)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Function (props)](#apidoc.element.uglifyjs.AST_Function)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Hole (props)](#apidoc.element.uglifyjs.AST_Hole)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_If (props)](#apidoc.element.uglifyjs.AST_If)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Infinity (props)](#apidoc.element.uglifyjs.AST_Infinity)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_IterationStatement (props)](#apidoc.element.uglifyjs.AST_IterationStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Jump (props)](#apidoc.element.uglifyjs.AST_Jump)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Label (props)](#apidoc.element.uglifyjs.AST_Label)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabelRef (props)](#apidoc.element.uglifyjs.AST_LabelRef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabeledStatement (props)](#apidoc.element.uglifyjs.AST_LabeledStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Lambda (props)](#apidoc.element.uglifyjs.AST_Lambda)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LoopControl (props)](#apidoc.element.uglifyjs.AST_LoopControl)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_NaN (props)](#apidoc.element.uglifyjs.AST_NaN)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_New (props)](#apidoc.element.uglifyjs.AST_New)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Node (props)](#apidoc.element.uglifyjs.AST_Node)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Null (props)](#apidoc.element.uglifyjs.AST_Null)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Number (props)](#apidoc.element.uglifyjs.AST_Number)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Object (props)](#apidoc.element.uglifyjs.AST_Object)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectGetter (props)](#apidoc.element.uglifyjs.AST_ObjectGetter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectProperty (props)](#apidoc.element.uglifyjs.AST_ObjectProperty)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectSetter (props)](#apidoc.element.uglifyjs.AST_ObjectSetter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_PropAccess (props)](#apidoc.element.uglifyjs.AST_PropAccess)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_RegExp (props)](#apidoc.element.uglifyjs.AST_RegExp)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Return (props)](#apidoc.element.uglifyjs.AST_Return)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Scope (props)](#apidoc.element.uglifyjs.AST_Scope)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Seq (props)](#apidoc.element.uglifyjs.AST_Seq)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SimpleStatement (props)](#apidoc.element.uglifyjs.AST_SimpleStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Statement (props)](#apidoc.element.uglifyjs.AST_Statement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_StatementWithBody (props)](#apidoc.element.uglifyjs.AST_StatementWithBody)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_String (props)](#apidoc.element.uglifyjs.AST_String)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Sub (props)](#apidoc.element.uglifyjs.AST_Sub)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Switch (props)](#apidoc.element.uglifyjs.AST_Switch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SwitchBranch (props)](#apidoc.element.uglifyjs.AST_SwitchBranch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Symbol (props)](#apidoc.element.uglifyjs.AST_Symbol)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolAccessor (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolCatch (props)](#apidoc.element.uglifyjs.AST_SymbolCatch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolConst (props)](#apidoc.element.uglifyjs.AST_SymbolConst)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDefun (props)](#apidoc.element.uglifyjs.AST_SymbolDefun)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolFunarg (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolLambda (props)](#apidoc.element.uglifyjs.AST_SymbolLambda)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolRef (props)](#apidoc.element.uglifyjs.AST_SymbolRef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolVar (props)](#apidoc.element.uglifyjs.AST_SymbolVar)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_This (props)](#apidoc.element.uglifyjs.AST_This)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Throw (props)](#apidoc.element.uglifyjs.AST_Throw)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Token (props)](#apidoc.element.uglifyjs.AST_Token)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Toplevel (props)](#apidoc.element.uglifyjs.AST_Toplevel)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_True (props)](#apidoc.element.uglifyjs.AST_True)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Try (props)](#apidoc.element.uglifyjs.AST_Try)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Unary (props)](#apidoc.element.uglifyjs.AST_Unary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPostfix (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPrefix (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Undefined (props)](#apidoc.element.uglifyjs.AST_Undefined)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Var (props)](#apidoc.element.uglifyjs.AST_Var)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_VarDef (props)](#apidoc.element.uglifyjs.AST_VarDef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_While (props)](#apidoc.element.uglifyjs.AST_While)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_With (props)](#apidoc.element.uglifyjs.AST_With)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.uglifyjs.Buffer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>Compressor (options, false_by_default)](#apidoc.element.uglifyjs.Compressor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>DEFNODE (type, props, methods, base)](#apidoc.element.uglifyjs.DEFNODE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>DefaultsError (msg, defs)](#apidoc.element.uglifyjs.DefaultsError)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>Dictionary ()](#apidoc.element.uglifyjs.Dictionary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglifyjs.JS_Parse_Error)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>KEYWORDS (str )](#apidoc.element.uglifyjs.KEYWORDS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>KEYWORDS_ATOM (str )](#apidoc.element.uglifyjs.KEYWORDS_ATOM)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>KEYWORDS_BEFORE_EXPRESSION (str )](#apidoc.element.uglifyjs.KEYWORDS_BEFORE_EXPRESSION)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>MAP (a, f, backwards)](#apidoc.element.uglifyjs.MAP)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceMapConsumer (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceMapGenerator (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceNode (aLine, aColumn, aSource, aChunks, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>OPERATORS (str )](#apidoc.element.uglifyjs.OPERATORS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>OPERATOR_CHARS (str )](#apidoc.element.uglifyjs.OPERATOR_CHARS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>OutputStream (options)](#apidoc.element.uglifyjs.OutputStream)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>PUNC_BEFORE_EXPRESSION (str )](#apidoc.element.uglifyjs.PUNC_BEFORE_EXPRESSION)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>PUNC_CHARS (str )](#apidoc.element.uglifyjs.PUNC_CHARS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>REGEXP_MODIFIERS (str )](#apidoc.element.uglifyjs.REGEXP_MODIFIERS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>RESERVED_WORDS (str )](#apidoc.element.uglifyjs.RESERVED_WORDS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>SourceMap (options)](#apidoc.element.uglifyjs.SourceMap)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglifyjs.SymbolDef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>TreeTransformer (before, after)](#apidoc.element.uglifyjs.TreeTransformer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>TreeWalker (callback)](#apidoc.element.uglifyjs.TreeWalker)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>UNARY_POSTFIX (str )](#apidoc.element.uglifyjs.UNARY_POSTFIX)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>UNARY_PREFIX (str )](#apidoc.element.uglifyjs.UNARY_PREFIX)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>WHITESPACE_CHARS (str )](#apidoc.element.uglifyjs.WHITESPACE_CHARS)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>all (array, predicate)](#apidoc.element.uglifyjs.all)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>array_to_hash (a)](#apidoc.element.uglifyjs.array_to_hash)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>base54 (num)](#apidoc.element.uglifyjs.base54)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>characters (str)](#apidoc.element.uglifyjs.characters)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>defaults (args, defs, croak)](#apidoc.element.uglifyjs.defaults)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>describe_ast ()](#apidoc.element.uglifyjs.describe_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>find_if (func, array)](#apidoc.element.uglifyjs.find_if)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_alphanumeric_char (code)](#apidoc.element.uglifyjs.is_alphanumeric_char)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_digit (code)](#apidoc.element.uglifyjs.is_digit)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier (name)](#apidoc.element.uglifyjs.is_identifier)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier_char (ch)](#apidoc.element.uglifyjs.is_identifier_char)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier_start (code)](#apidoc.element.uglifyjs.is_identifier_start)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier_string (str)](#apidoc.element.uglifyjs.is_identifier_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_letter (code)](#apidoc.element.uglifyjs.is_letter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_token (token, type, val)](#apidoc.element.uglifyjs.is_token)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_unicode_combining_mark (ch)](#apidoc.element.uglifyjs.is_unicode_combining_mark)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_unicode_connector_punctuation (ch)](#apidoc.element.uglifyjs.is_unicode_connector_punctuation)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>is_unicode_digit (code)](#apidoc.element.uglifyjs.is_unicode_digit)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>js_error (message, filename, line, col, pos)](#apidoc.element.uglifyjs.js_error)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>makePredicate (words)](#apidoc.element.uglifyjs.makePredicate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>member (name, array)](#apidoc.element.uglifyjs.member)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>merge (obj, ext)](#apidoc.element.uglifyjs.merge)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>mergeSort (array, cmp)](#apidoc.element.uglifyjs.mergeSort)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>minify (files, options)](#apidoc.element.uglifyjs.minify)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>noop ()](#apidoc.element.uglifyjs.noop)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>parse ($TEXT, options)](#apidoc.element.uglifyjs.parse)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>parse_js_number (num)](#apidoc.element.uglifyjs.parse_js_number)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>push_uniq (array, el)](#apidoc.element.uglifyjs.push_uniq)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>remove (array, el)](#apidoc.element.uglifyjs.remove)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>repeat_string (str, i)](#apidoc.element.uglifyjs.repeat_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>set_difference (a, b)](#apidoc.element.uglifyjs.set_difference)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>set_intersection (a, b)](#apidoc.element.uglifyjs.set_intersection)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>slice (a, start)](#apidoc.element.uglifyjs.slice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>string_template (text, props)](#apidoc.element.uglifyjs.string_template)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>tokenizer ($TEXT, filename, html5_comments)](#apidoc.element.uglifyjs.tokenizer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>walk_body (node, visitor)](#apidoc.element.uglifyjs.walk_body)
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Accessor.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Array.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Assign.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Atom.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Atom.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Binary.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Binary.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Block.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Block.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_BlockStatement.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Boolean.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Boolean.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Break.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Call.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Call.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Case.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Catch.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Conditional.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Const.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Constant.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Constant.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Continue.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_DWLoop.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_DWLoop.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Debugger.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Default.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Definitions.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Definitions.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Defun.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Directive.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Do.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Dot.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_EmptyStatement.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Exit.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Exit.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_False.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Finally.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_For.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_ForIn.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Function.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Hole.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_If.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Infinity.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_IterationStatement.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_IterationStatement.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Jump.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Jump.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Label.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabelRef.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabeledStatement.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Lambda.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Lambda.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_LoopControl.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_LoopControl.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_NaN.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_New.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Node.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Node.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Null.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Number.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Object.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectGetter.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectKeyVal.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectProperty.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectProperty.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectSetter.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_PropAccess.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_PropAccess.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_RegExp.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Return.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Scope.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Scope.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Seq.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SimpleStatement.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Statement.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Statement.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_StatementWithBody.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_StatementWithBody.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_String.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Sub.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Switch.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SwitchBranch.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SwitchBranch.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Symbol.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Symbol.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolAccessor.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolCatch.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolConst.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDeclaration.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDeclaration.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDefun.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolFunarg.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolLambda.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolRef.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolVar.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolVar.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_This.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Throw.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Token.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Toplevel.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_True.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Try.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Unary.SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Unary.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPostfix.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPrefix.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Undefined.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_Var.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_VarDef.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_While.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>AST_With.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>ATOMIC_START_TOKEN
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>Buffer.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>Compressor.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>DefaultsError.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>Dictionary.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>EX_EOF
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>FILES
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>JS_Parse_Error.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceMapConsumer.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceMapGenerator.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceNode.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>PRECEDENCE
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>RE_DEC_NUMBER
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>RE_HEX_NUMBER
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>RE_OCT_NUMBER
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>STATEMENTS_WITH_LABELS
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>SymbolDef.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>TreeWalker.prototype
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>UNICODE
1.  object <span class="apidocSignatureSpan">uglifyjs.</span>sys

#### [module uglifyjs.AST_Accessor](#apidoc.module.uglifyjs.AST_Accessor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Accessor (props)](#apidoc.element.uglifyjs.AST_Accessor.AST_Accessor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Accessor.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Accessor.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>documentation

#### [module uglifyjs.AST_Accessor.prototype](#apidoc.module.uglifyjs.AST_Accessor.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Accessor.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.prototype.</span>TYPE

#### [module uglifyjs.AST_Array](#apidoc.module.uglifyjs.AST_Array)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Array (props)](#apidoc.element.uglifyjs.AST_Array.AST_Array)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Array.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Array.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>documentation

#### [module uglifyjs.AST_Array.prototype](#apidoc.module.uglifyjs.AST_Array.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Array.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Array.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Array.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Array.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Array.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Array.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Array.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>TYPE

#### [module uglifyjs.AST_Assign](#apidoc.module.uglifyjs.AST_Assign)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Assign (props)](#apidoc.element.uglifyjs.AST_Assign.AST_Assign)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Assign.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Assign.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>documentation

#### [module uglifyjs.AST_Assign.prototype](#apidoc.module.uglifyjs.AST_Assign.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Assign.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Assign.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Assign.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Assign.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Assign.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Assign.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Assign.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>TYPE

#### [module uglifyjs.AST_Atom](#apidoc.module.uglifyjs.AST_Atom)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Atom (props)](#apidoc.element.uglifyjs.AST_Atom.AST_Atom)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Atom.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Atom.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>documentation

#### [module uglifyjs.AST_Atom.SUBCLASSES](#apidoc.module.uglifyjs.AST_Atom.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.5)

#### [module uglifyjs.AST_Atom.prototype](#apidoc.module.uglifyjs.AST_Atom.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Atom.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Atom.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Atom.prototype.</span>TYPE

#### [module uglifyjs.AST_Binary](#apidoc.module.uglifyjs.AST_Binary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Binary (props)](#apidoc.element.uglifyjs.AST_Binary.AST_Binary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Binary.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Binary.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>documentation

#### [module uglifyjs.AST_Binary.SUBCLASSES](#apidoc.module.uglifyjs.AST_Binary.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Binary.SUBCLASSES.0)

#### [module uglifyjs.AST_Binary.prototype](#apidoc.module.uglifyjs.AST_Binary.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Binary.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Binary.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>_eval (c)](#apidoc.element.uglifyjs.AST_Binary.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Binary.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Binary.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.lift_sequences)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Binary.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Binary.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Binary.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>TYPE

#### [module uglifyjs.AST_Block](#apidoc.module.uglifyjs.AST_Block)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Block (props)](#apidoc.element.uglifyjs.AST_Block.AST_Block)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Block.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Block.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>documentation

#### [module uglifyjs.AST_Block.SUBCLASSES](#apidoc.module.uglifyjs.AST_Block.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.5)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>6 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.6)

#### [module uglifyjs.AST_Block.prototype](#apidoc.module.uglifyjs.AST_Block.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Block.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Block.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Block.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Block.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Block.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Block.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>TYPE

#### [module uglifyjs.AST_BlockStatement](#apidoc.module.uglifyjs.AST_BlockStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_BlockStatement (props)](#apidoc.element.uglifyjs.AST_BlockStatement.AST_BlockStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_BlockStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_BlockStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>documentation

#### [module uglifyjs.AST_BlockStatement.prototype](#apidoc.module.uglifyjs.AST_BlockStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>TYPE

#### [module uglifyjs.AST_Boolean](#apidoc.module.uglifyjs.AST_Boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Boolean (props)](#apidoc.element.uglifyjs.AST_Boolean.AST_Boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Boolean.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Boolean.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>documentation

#### [module uglifyjs.AST_Boolean.SUBCLASSES](#apidoc.module.uglifyjs.AST_Boolean.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Boolean.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Boolean.SUBCLASSES.1)

#### [module uglifyjs.AST_Boolean.prototype](#apidoc.module.uglifyjs.AST_Boolean.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Boolean.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Boolean.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Boolean.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>TYPE

#### [module uglifyjs.AST_Break](#apidoc.module.uglifyjs.AST_Break)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Break (props)](#apidoc.element.uglifyjs.AST_Break.AST_Break)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Break.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Break.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>documentation

#### [module uglifyjs.AST_Break.prototype](#apidoc.module.uglifyjs.AST_Break.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Break.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Break.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Break.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>TYPE

#### [module uglifyjs.AST_Call](#apidoc.module.uglifyjs.AST_Call)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Call (props)](#apidoc.element.uglifyjs.AST_Call.AST_Call)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Call.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Call.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>documentation

#### [module uglifyjs.AST_Call.SUBCLASSES](#apidoc.module.uglifyjs.AST_Call.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Call.SUBCLASSES.0)

#### [module uglifyjs.AST_Call.prototype](#apidoc.module.uglifyjs.AST_Call.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Call.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Call.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Call.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Call.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Call.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Call.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Call.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Call.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Call.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>TYPE

#### [module uglifyjs.AST_Case](#apidoc.module.uglifyjs.AST_Case)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Case (props)](#apidoc.element.uglifyjs.AST_Case.AST_Case)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Case.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Case.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>documentation

#### [module uglifyjs.AST_Case.prototype](#apidoc.module.uglifyjs.AST_Case.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Case.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Case.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Case.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Case.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Case.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>TYPE

#### [module uglifyjs.AST_Catch](#apidoc.module.uglifyjs.AST_Catch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Catch (props)](#apidoc.element.uglifyjs.AST_Catch.AST_Catch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Catch.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Catch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>documentation

#### [module uglifyjs.AST_Catch.prototype](#apidoc.module.uglifyjs.AST_Catch.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Catch.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Catch.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Catch.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Catch.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Catch.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Catch.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>TYPE

#### [module uglifyjs.AST_Conditional](#apidoc.module.uglifyjs.AST_Conditional)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Conditional (props)](#apidoc.element.uglifyjs.AST_Conditional.AST_Conditional)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Conditional.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Conditional.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>documentation

#### [module uglifyjs.AST_Conditional.prototype](#apidoc.module.uglifyjs.AST_Conditional.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Conditional.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Conditional.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Conditional.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Conditional.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Conditional.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Conditional.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Conditional.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>TYPE

#### [module uglifyjs.AST_Const](#apidoc.module.uglifyjs.AST_Const)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Const (props)](#apidoc.element.uglifyjs.AST_Const.AST_Const)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Const.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Const.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>documentation

#### [module uglifyjs.AST_Const.prototype](#apidoc.module.uglifyjs.AST_Const.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Const.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Const.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Const.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Const.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Const.prototype.</span>TYPE

#### [module uglifyjs.AST_Constant](#apidoc.module.uglifyjs.AST_Constant)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Constant (props)](#apidoc.element.uglifyjs.AST_Constant.AST_Constant)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Constant.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Constant.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>documentation

#### [module uglifyjs.AST_Constant.SUBCLASSES](#apidoc.module.uglifyjs.AST_Constant.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.3)

#### [module uglifyjs.AST_Constant.prototype](#apidoc.module.uglifyjs.AST_Constant.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Constant.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Constant.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Constant.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Constant.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>getValue ()](#apidoc.element.uglifyjs.AST_Constant.prototype.getValue)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Constant.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Constant.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>TYPE

#### [module uglifyjs.AST_Continue](#apidoc.module.uglifyjs.AST_Continue)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Continue (props)](#apidoc.element.uglifyjs.AST_Continue.AST_Continue)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Continue.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Continue.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>documentation

#### [module uglifyjs.AST_Continue.prototype](#apidoc.module.uglifyjs.AST_Continue.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Continue.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Continue.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Continue.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>TYPE

#### [module uglifyjs.AST_DWLoop](#apidoc.module.uglifyjs.AST_DWLoop)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_DWLoop (props)](#apidoc.element.uglifyjs.AST_DWLoop.AST_DWLoop)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>BASE (props)](#apidoc.element.uglifyjs.AST_DWLoop.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_DWLoop.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>documentation

#### [module uglifyjs.AST_DWLoop.SUBCLASSES](#apidoc.module.uglifyjs.AST_DWLoop.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_DWLoop.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_DWLoop.SUBCLASSES.1)

#### [module uglifyjs.AST_DWLoop.prototype](#apidoc.module.uglifyjs.AST_DWLoop.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_DWLoop.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_DWLoop.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_DWLoop.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>TYPE

#### [module uglifyjs.AST_Debugger](#apidoc.module.uglifyjs.AST_Debugger)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Debugger (props)](#apidoc.element.uglifyjs.AST_Debugger.AST_Debugger)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Debugger.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Debugger.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>documentation

#### [module uglifyjs.AST_Debugger.prototype](#apidoc.module.uglifyjs.AST_Debugger.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Debugger.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Debugger.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Debugger.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Debugger.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Debugger.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>TYPE

#### [module uglifyjs.AST_Default](#apidoc.module.uglifyjs.AST_Default)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Default (props)](#apidoc.element.uglifyjs.AST_Default.AST_Default)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Default.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Default.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>documentation

#### [module uglifyjs.AST_Default.prototype](#apidoc.module.uglifyjs.AST_Default.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Default.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Default.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Default.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Default.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Default.prototype.</span>TYPE

#### [module uglifyjs.AST_Definitions](#apidoc.module.uglifyjs.AST_Definitions)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Definitions (props)](#apidoc.element.uglifyjs.AST_Definitions.AST_Definitions)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Definitions.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Definitions.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>documentation

#### [module uglifyjs.AST_Definitions.SUBCLASSES](#apidoc.module.uglifyjs.AST_Definitions.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Definitions.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Definitions.SUBCLASSES.1)

#### [module uglifyjs.AST_Definitions.prototype](#apidoc.module.uglifyjs.AST_Definitions.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Definitions.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>_do_print (output, kind)](#apidoc.element.uglifyjs.AST_Definitions.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Definitions.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Definitions.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Definitions.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>remove_initializers ()](#apidoc.element.uglifyjs.AST_Definitions.prototype.remove_initializers)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>to_assignments ()](#apidoc.element.uglifyjs.AST_Definitions.prototype.to_assignments)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Definitions.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Definitions.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>TYPE

#### [module uglifyjs.AST_Defun](#apidoc.module.uglifyjs.AST_Defun)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Defun (props)](#apidoc.element.uglifyjs.AST_Defun.AST_Defun)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Defun.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Defun.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>documentation

#### [module uglifyjs.AST_Defun.prototype](#apidoc.module.uglifyjs.AST_Defun.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Defun.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Defun.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Defun.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>TYPE

#### [module uglifyjs.AST_Directive](#apidoc.module.uglifyjs.AST_Directive)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Directive (props)](#apidoc.element.uglifyjs.AST_Directive.AST_Directive)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Directive.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Directive.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>documentation

#### [module uglifyjs.AST_Directive.prototype](#apidoc.module.uglifyjs.AST_Directive.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Directive.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Directive.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Directive.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Directive.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Directive.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>TYPE

#### [module uglifyjs.AST_Do](#apidoc.module.uglifyjs.AST_Do)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Do (props)](#apidoc.element.uglifyjs.AST_Do.AST_Do)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Do.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Do.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>documentation

#### [module uglifyjs.AST_Do.prototype](#apidoc.module.uglifyjs.AST_Do.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Do.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Do.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Do.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Do.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>TYPE

#### [module uglifyjs.AST_Dot](#apidoc.module.uglifyjs.AST_Dot)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Dot (props)](#apidoc.element.uglifyjs.AST_Dot.AST_Dot)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Dot.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Dot.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>documentation

#### [module uglifyjs.AST_Dot.prototype](#apidoc.module.uglifyjs.AST_Dot.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Dot.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Dot.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_Dot.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Dot.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Dot.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Dot.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Dot.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>TYPE

#### [module uglifyjs.AST_EmptyStatement](#apidoc.module.uglifyjs.AST_EmptyStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_EmptyStatement (props)](#apidoc.element.uglifyjs.AST_EmptyStatement.AST_EmptyStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_EmptyStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_EmptyStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>documentation

#### [module uglifyjs.AST_EmptyStatement.prototype](#apidoc.module.uglifyjs.AST_EmptyStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>TYPE

#### [module uglifyjs.AST_Exit](#apidoc.module.uglifyjs.AST_Exit)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Exit (props)](#apidoc.element.uglifyjs.AST_Exit.AST_Exit)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Exit.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Exit.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>documentation

#### [module uglifyjs.AST_Exit.SUBCLASSES](#apidoc.module.uglifyjs.AST_Exit.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Exit.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Exit.SUBCLASSES.1)

#### [module uglifyjs.AST_Exit.prototype](#apidoc.module.uglifyjs.AST_Exit.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Exit.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>_do_print (output, kind)](#apidoc.element.uglifyjs.AST_Exit.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Exit.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Exit.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>TYPE

#### [module uglifyjs.AST_False](#apidoc.module.uglifyjs.AST_False)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_False (props)](#apidoc.element.uglifyjs.AST_False.AST_False)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>BASE (props)](#apidoc.element.uglifyjs.AST_False.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_False.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>documentation

#### [module uglifyjs.AST_False.prototype](#apidoc.module.uglifyjs.AST_False.prototype)
1.  boolean <span class="apidocSignatureSpan">uglifyjs.AST_False.prototype.</span>value
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_False.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_False.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_False.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_False.prototype.is_boolean)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_False.prototype.</span>TYPE

#### [module uglifyjs.AST_Finally](#apidoc.module.uglifyjs.AST_Finally)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Finally (props)](#apidoc.element.uglifyjs.AST_Finally.AST_Finally)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Finally.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Finally.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>documentation

#### [module uglifyjs.AST_Finally.prototype](#apidoc.module.uglifyjs.AST_Finally.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Finally.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Finally.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Finally.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>TYPE

#### [module uglifyjs.AST_For](#apidoc.module.uglifyjs.AST_For)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_For (props)](#apidoc.element.uglifyjs.AST_For.AST_For)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>BASE (props)](#apidoc.element.uglifyjs.AST_For.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_For.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>documentation

#### [module uglifyjs.AST_For.prototype](#apidoc.module.uglifyjs.AST_For.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_For.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_For.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_For.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_For.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_For.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_For.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>TYPE

#### [module uglifyjs.AST_ForIn](#apidoc.module.uglifyjs.AST_ForIn)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ForIn (props)](#apidoc.element.uglifyjs.AST_ForIn.AST_ForIn)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ForIn.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ForIn.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>documentation

#### [module uglifyjs.AST_ForIn.prototype](#apidoc.module.uglifyjs.AST_ForIn.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ForIn.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ForIn.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_ForIn.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_ForIn.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_ForIn.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>TYPE

#### [module uglifyjs.AST_Function](#apidoc.module.uglifyjs.AST_Function)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Function (props)](#apidoc.element.uglifyjs.AST_Function.AST_Function)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Function.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Function.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>documentation

#### [module uglifyjs.AST_Function.prototype](#apidoc.module.uglifyjs.AST_Function.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Function.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Function.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Function.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Function.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Function.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>next_mangled (options, def)](#apidoc.element.uglifyjs.AST_Function.prototype.next_mangled)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Function.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Function.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>TYPE

#### [module uglifyjs.AST_Hole](#apidoc.module.uglifyjs.AST_Hole)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Hole (props)](#apidoc.element.uglifyjs.AST_Hole.AST_Hole)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Hole.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Hole.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>documentation

#### [module uglifyjs.AST_Hole.prototype](#apidoc.module.uglifyjs.AST_Hole.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Hole.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>_codegen ()](#apidoc.element.uglifyjs.AST_Hole.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Hole.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>TYPE

#### [module uglifyjs.AST_If](#apidoc.module.uglifyjs.AST_If)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_If (props)](#apidoc.element.uglifyjs.AST_If.AST_If)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>BASE (props)](#apidoc.element.uglifyjs.AST_If.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_If.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>documentation

#### [module uglifyjs.AST_If.prototype](#apidoc.module.uglifyjs.AST_If.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_If.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_If.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_If.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_If.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_If.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_If.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_If.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>TYPE

#### [module uglifyjs.AST_Infinity](#apidoc.module.uglifyjs.AST_Infinity)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Infinity (props)](#apidoc.element.uglifyjs.AST_Infinity.AST_Infinity)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Infinity.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Infinity.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>documentation

#### [module uglifyjs.AST_Infinity.prototype](#apidoc.module.uglifyjs.AST_Infinity.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Infinity.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Infinity.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Infinity.prototype.optimize)
1.  number <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>value
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>TYPE

#### [module uglifyjs.AST_IterationStatement](#apidoc.module.uglifyjs.AST_IterationStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_IterationStatement (props)](#apidoc.element.uglifyjs.AST_IterationStatement.AST_IterationStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_IterationStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_IterationStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>documentation

#### [module uglifyjs.AST_IterationStatement.SUBCLASSES](#apidoc.module.uglifyjs.AST_IterationStatement.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.2)

#### [module uglifyjs.AST_IterationStatement.prototype](#apidoc.module.uglifyjs.AST_IterationStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_IterationStatement.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.prototype.</span>TYPE

#### [module uglifyjs.AST_Jump](#apidoc.module.uglifyjs.AST_Jump)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Jump (props)](#apidoc.element.uglifyjs.AST_Jump.AST_Jump)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Jump.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Jump.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>documentation

#### [module uglifyjs.AST_Jump.SUBCLASSES](#apidoc.module.uglifyjs.AST_Jump.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Jump.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Jump.SUBCLASSES.1)

#### [module uglifyjs.AST_Jump.prototype](#apidoc.module.uglifyjs.AST_Jump.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Jump.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_Jump.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Jump.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>TYPE

#### [module uglifyjs.AST_Label](#apidoc.module.uglifyjs.AST_Label)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Label (props)](#apidoc.element.uglifyjs.AST_Label.AST_Label)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Label.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Label.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>documentation

#### [module uglifyjs.AST_Label.prototype](#apidoc.module.uglifyjs.AST_Label.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Label.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>initialize ()](#apidoc.element.uglifyjs.AST_Label.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>undeclared ()](#apidoc.element.uglifyjs.AST_Label.prototype.undeclared)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>unmangleable ()](#apidoc.element.uglifyjs.AST_Label.prototype.unmangleable)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>TYPE

#### [module uglifyjs.AST_LabelRef](#apidoc.module.uglifyjs.AST_LabelRef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabelRef (props)](#apidoc.element.uglifyjs.AST_LabelRef.AST_LabelRef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>BASE (props)](#apidoc.element.uglifyjs.AST_LabelRef.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_LabelRef.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>documentation

#### [module uglifyjs.AST_LabelRef.prototype](#apidoc.module.uglifyjs.AST_LabelRef.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_LabelRef.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.prototype.</span>undeclared ()](#apidoc.element.uglifyjs.AST_LabelRef.prototype.undeclared)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.prototype.</span>TYPE

#### [module uglifyjs.AST_LabeledStatement](#apidoc.module.uglifyjs.AST_LabeledStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabeledStatement (props)](#apidoc.element.uglifyjs.AST_LabeledStatement.AST_LabeledStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_LabeledStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_LabeledStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>documentation

#### [module uglifyjs.AST_LabeledStatement.prototype](#apidoc.module.uglifyjs.AST_LabeledStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>TYPE

#### [module uglifyjs.AST_Lambda](#apidoc.module.uglifyjs.AST_Lambda)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Lambda (props)](#apidoc.element.uglifyjs.AST_Lambda.AST_Lambda)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Lambda.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Lambda.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>documentation

#### [module uglifyjs.AST_Lambda.SUBCLASSES](#apidoc.module.uglifyjs.AST_Lambda.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.2)

#### [module uglifyjs.AST_Lambda.prototype](#apidoc.module.uglifyjs.AST_Lambda.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Lambda.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Lambda.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>_do_print (output, nokeyword)](#apidoc.element.uglifyjs.AST_Lambda.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Lambda.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Lambda.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>init_scope_vars ()](#apidoc.element.uglifyjs.AST_Lambda.prototype.init_scope_vars)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Lambda.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Lambda.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>TYPE

#### [module uglifyjs.AST_LoopControl](#apidoc.module.uglifyjs.AST_LoopControl)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LoopControl (props)](#apidoc.element.uglifyjs.AST_LoopControl.AST_LoopControl)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>BASE (props)](#apidoc.element.uglifyjs.AST_LoopControl.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_LoopControl.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>documentation

#### [module uglifyjs.AST_LoopControl.SUBCLASSES](#apidoc.module.uglifyjs.AST_LoopControl.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_LoopControl.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_LoopControl.SUBCLASSES.1)

#### [module uglifyjs.AST_LoopControl.prototype](#apidoc.module.uglifyjs.AST_LoopControl.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_LoopControl.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>_do_print (output, kind)](#apidoc.element.uglifyjs.AST_LoopControl.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_LoopControl.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_LoopControl.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>TYPE

#### [module uglifyjs.AST_NaN](#apidoc.module.uglifyjs.AST_NaN)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_NaN (props)](#apidoc.element.uglifyjs.AST_NaN.AST_NaN)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>BASE (props)](#apidoc.element.uglifyjs.AST_NaN.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_NaN.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>documentation

#### [module uglifyjs.AST_NaN.prototype](#apidoc.module.uglifyjs.AST_NaN.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_NaN.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_NaN.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_NaN.prototype.optimize)
1.  number <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>value
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>TYPE

#### [module uglifyjs.AST_New](#apidoc.module.uglifyjs.AST_New)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_New (props)](#apidoc.element.uglifyjs.AST_New.AST_New)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>BASE (props)](#apidoc.element.uglifyjs.AST_New.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_New.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>documentation

#### [module uglifyjs.AST_New.prototype](#apidoc.module.uglifyjs.AST_New.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_New.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_New.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_New.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_New.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_New.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_New.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>TYPE

#### [module uglifyjs.AST_Node](#apidoc.module.uglifyjs.AST_Node)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Node (props)](#apidoc.element.uglifyjs.AST_Node.AST_Node)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Node.DEFMETHOD)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>from_mozilla_ast (node)](#apidoc.element.uglifyjs.AST_Node.from_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>warn (txt, props)](#apidoc.element.uglifyjs.AST_Node.warn)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>warn_function (txt)](#apidoc.element.uglifyjs.AST_Node.warn_function)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>documentation

#### [module uglifyjs.AST_Node.SUBCLASSES](#apidoc.module.uglifyjs.AST_Node.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>10 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.10)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>11 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.11)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>12 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.12)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.5)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>6 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.6)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>7 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.7)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>8 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.8)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>9 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.9)

#### [module uglifyjs.AST_Node.prototype](#apidoc.module.uglifyjs.AST_Node.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Node.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Node.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Node.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>add_comments (output)](#apidoc.element.uglifyjs.AST_Node.prototype.add_comments)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Node.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>clone ()](#apidoc.element.uglifyjs.AST_Node.prototype.clone)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>equivalent_to (node)](#apidoc.element.uglifyjs.AST_Node.prototype.equivalent_to)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>evaluate (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.evaluate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Node.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>is_string ()](#apidoc.element.uglifyjs.AST_Node.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>needs_parens ()](#apidoc.element.uglifyjs.AST_Node.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>print (stream, force_parens)](#apidoc.element.uglifyjs.AST_Node.prototype.print)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>print_to_string (options)](#apidoc.element.uglifyjs.AST_Node.prototype.print_to_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Node.prototype.transform)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>walk (visitor)](#apidoc.element.uglifyjs.AST_Node.prototype.walk)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>TYPE

#### [module uglifyjs.AST_Null](#apidoc.module.uglifyjs.AST_Null)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Null (props)](#apidoc.element.uglifyjs.AST_Null.AST_Null)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Null.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Null.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>documentation

#### [module uglifyjs.AST_Null.prototype](#apidoc.module.uglifyjs.AST_Null.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Null.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Null.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Null.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Null.prototype.to_mozilla_ast)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Null.prototype.</span>value
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Null.prototype.</span>TYPE

#### [module uglifyjs.AST_Number](#apidoc.module.uglifyjs.AST_Number)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Number (props)](#apidoc.element.uglifyjs.AST_Number.AST_Number)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Number.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Number.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>documentation

#### [module uglifyjs.AST_Number.prototype](#apidoc.module.uglifyjs.AST_Number.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Number.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Number.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Number.prototype.needs_parens)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>TYPE

#### [module uglifyjs.AST_Object](#apidoc.module.uglifyjs.AST_Object)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Object (props)](#apidoc.element.uglifyjs.AST_Object.AST_Object)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Object.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Object.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>documentation

#### [module uglifyjs.AST_Object.prototype](#apidoc.module.uglifyjs.AST_Object.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Object.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Object.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Object.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Object.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Object.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Object.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Object.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Object.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>TYPE

#### [module uglifyjs.AST_ObjectGetter](#apidoc.module.uglifyjs.AST_ObjectGetter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectGetter (props)](#apidoc.element.uglifyjs.AST_ObjectGetter.AST_ObjectGetter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectGetter.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectGetter.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>documentation

#### [module uglifyjs.AST_ObjectGetter.prototype](#apidoc.module.uglifyjs.AST_ObjectGetter.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectGetter.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ObjectGetter.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.prototype.</span>TYPE

#### [module uglifyjs.AST_ObjectKeyVal](#apidoc.module.uglifyjs.AST_ObjectKeyVal)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.AST_ObjectKeyVal)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>documentation

#### [module uglifyjs.AST_ObjectKeyVal.prototype](#apidoc.module.uglifyjs.AST_ObjectKeyVal.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.prototype.</span>TYPE

#### [module uglifyjs.AST_ObjectProperty](#apidoc.module.uglifyjs.AST_ObjectProperty)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectProperty (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.AST_ObjectProperty)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectProperty.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>documentation

#### [module uglifyjs.AST_ObjectProperty.SUBCLASSES](#apidoc.module.uglifyjs.AST_ObjectProperty.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.2)

#### [module uglifyjs.AST_ObjectProperty.prototype](#apidoc.module.uglifyjs.AST_ObjectProperty.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>TYPE

#### [module uglifyjs.AST_ObjectSetter](#apidoc.module.uglifyjs.AST_ObjectSetter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectSetter (props)](#apidoc.element.uglifyjs.AST_ObjectSetter.AST_ObjectSetter)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectSetter.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectSetter.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>documentation

#### [module uglifyjs.AST_ObjectSetter.prototype](#apidoc.module.uglifyjs.AST_ObjectSetter.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectSetter.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ObjectSetter.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.prototype.</span>TYPE

#### [module uglifyjs.AST_PropAccess](#apidoc.module.uglifyjs.AST_PropAccess)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_PropAccess (props)](#apidoc.element.uglifyjs.AST_PropAccess.AST_PropAccess)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>BASE (props)](#apidoc.element.uglifyjs.AST_PropAccess.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_PropAccess.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>documentation

#### [module uglifyjs.AST_PropAccess.SUBCLASSES](#apidoc.module.uglifyjs.AST_PropAccess.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_PropAccess.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_PropAccess.SUBCLASSES.1)

#### [module uglifyjs.AST_PropAccess.prototype](#apidoc.module.uglifyjs.AST_PropAccess.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_PropAccess.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_PropAccess.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_PropAccess.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_PropAccess.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>TYPE

#### [module uglifyjs.AST_RegExp](#apidoc.module.uglifyjs.AST_RegExp)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_RegExp (props)](#apidoc.element.uglifyjs.AST_RegExp.AST_RegExp)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>BASE (props)](#apidoc.element.uglifyjs.AST_RegExp.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_RegExp.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>documentation

#### [module uglifyjs.AST_RegExp.prototype](#apidoc.module.uglifyjs.AST_RegExp.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_RegExp.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_RegExp.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_RegExp.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>TYPE

#### [module uglifyjs.AST_Return](#apidoc.module.uglifyjs.AST_Return)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Return (props)](#apidoc.element.uglifyjs.AST_Return.AST_Return)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Return.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Return.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>documentation

#### [module uglifyjs.AST_Return.prototype](#apidoc.module.uglifyjs.AST_Return.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Return.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Return.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Return.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>TYPE

#### [module uglifyjs.AST_Scope](#apidoc.module.uglifyjs.AST_Scope)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Scope (props)](#apidoc.element.uglifyjs.AST_Scope.AST_Scope)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Scope.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Scope.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>documentation

#### [module uglifyjs.AST_Scope.SUBCLASSES](#apidoc.module.uglifyjs.AST_Scope.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Scope.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Scope.SUBCLASSES.1)

#### [module uglifyjs.AST_Scope.prototype](#apidoc.module.uglifyjs.AST_Scope.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Scope.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>def_function (symbol)](#apidoc.element.uglifyjs.AST_Scope.prototype.def_function)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>def_variable (symbol)](#apidoc.element.uglifyjs.AST_Scope.prototype.def_variable)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>drop_unused (compressor)](#apidoc.element.uglifyjs.AST_Scope.prototype.drop_unused)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>find_variable (name)](#apidoc.element.uglifyjs.AST_Scope.prototype.find_variable)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>has_directive (value)](#apidoc.element.uglifyjs.AST_Scope.prototype.has_directive)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>hoist_declarations (compressor)](#apidoc.element.uglifyjs.AST_Scope.prototype.hoist_declarations)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>init_scope_vars (nesting)](#apidoc.element.uglifyjs.AST_Scope.prototype.init_scope_vars)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>next_mangled (options)](#apidoc.element.uglifyjs.AST_Scope.prototype.next_mangled)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>references (sym)](#apidoc.element.uglifyjs.AST_Scope.prototype.references)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>strict ()](#apidoc.element.uglifyjs.AST_Scope.prototype.strict)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>TYPE

#### [module uglifyjs.AST_Seq](#apidoc.module.uglifyjs.AST_Seq)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Seq (props)](#apidoc.element.uglifyjs.AST_Seq.AST_Seq)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Seq.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Seq.DEFMETHOD)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>cons (x, y)](#apidoc.element.uglifyjs.AST_Seq.cons)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>from_array (array)](#apidoc.element.uglifyjs.AST_Seq.from_array)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>documentation

#### [module uglifyjs.AST_Seq.prototype](#apidoc.module.uglifyjs.AST_Seq.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Seq.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Seq.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>_do_print (output)](#apidoc.element.uglifyjs.AST_Seq.prototype._do_print)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Seq.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>add (node)](#apidoc.element.uglifyjs.AST_Seq.prototype.add)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Seq.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Seq.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>to_array ()](#apidoc.element.uglifyjs.AST_Seq.prototype.to_array)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Seq.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Seq.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>TYPE

#### [module uglifyjs.AST_SimpleStatement](#apidoc.module.uglifyjs.AST_SimpleStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SimpleStatement (props)](#apidoc.element.uglifyjs.AST_SimpleStatement.AST_SimpleStatement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SimpleStatement.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SimpleStatement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>documentation

#### [module uglifyjs.AST_SimpleStatement.prototype](#apidoc.module.uglifyjs.AST_SimpleStatement.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>TYPE

#### [module uglifyjs.AST_Statement](#apidoc.module.uglifyjs.AST_Statement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Statement (props)](#apidoc.element.uglifyjs.AST_Statement.AST_Statement)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Statement.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Statement.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>documentation

#### [module uglifyjs.AST_Statement.SUBCLASSES](#apidoc.module.uglifyjs.AST_Statement.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.5)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>6 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.6)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>7 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.7)

#### [module uglifyjs.AST_Statement.prototype](#apidoc.module.uglifyjs.AST_Statement.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Statement.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Statement.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Statement.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_Statement.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Statement.prototype.negate)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>TYPE

#### [module uglifyjs.AST_StatementWithBody](#apidoc.module.uglifyjs.AST_StatementWithBody)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_StatementWithBody (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.AST_StatementWithBody)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>BASE (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_StatementWithBody.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>documentation

#### [module uglifyjs.AST_StatementWithBody.SUBCLASSES](#apidoc.module.uglifyjs.AST_StatementWithBody.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.3)

#### [module uglifyjs.AST_StatementWithBody.prototype](#apidoc.module.uglifyjs.AST_StatementWithBody.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>_do_print_body (output)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype._do_print_body)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype.add_source_map)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>TYPE

#### [module uglifyjs.AST_String](#apidoc.module.uglifyjs.AST_String)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_String (props)](#apidoc.element.uglifyjs.AST_String.AST_String)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>BASE (props)](#apidoc.element.uglifyjs.AST_String.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_String.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>documentation

#### [module uglifyjs.AST_String.prototype](#apidoc.module.uglifyjs.AST_String.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_String.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_String.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>is_string ()](#apidoc.element.uglifyjs.AST_String.prototype.is_string)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>TYPE

#### [module uglifyjs.AST_Sub](#apidoc.module.uglifyjs.AST_Sub)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Sub (props)](#apidoc.element.uglifyjs.AST_Sub.AST_Sub)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Sub.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Sub.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>documentation

#### [module uglifyjs.AST_Sub.prototype](#apidoc.module.uglifyjs.AST_Sub.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Sub.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Sub.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Sub.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Sub.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Sub.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Sub.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>TYPE

#### [module uglifyjs.AST_Switch](#apidoc.module.uglifyjs.AST_Switch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Switch (props)](#apidoc.element.uglifyjs.AST_Switch.AST_Switch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Switch.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Switch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>documentation

#### [module uglifyjs.AST_Switch.prototype](#apidoc.module.uglifyjs.AST_Switch.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Switch.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Switch.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Switch.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Switch.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Switch.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Switch.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Switch.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>TYPE

#### [module uglifyjs.AST_SwitchBranch](#apidoc.module.uglifyjs.AST_SwitchBranch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SwitchBranch (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.AST_SwitchBranch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SwitchBranch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>documentation

#### [module uglifyjs.AST_SwitchBranch.SUBCLASSES](#apidoc.module.uglifyjs.AST_SwitchBranch.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.SUBCLASSES.1)

#### [module uglifyjs.AST_SwitchBranch.prototype](#apidoc.module.uglifyjs.AST_SwitchBranch.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>_do_print_body (output)](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype._do_print_body)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.aborts)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>TYPE

#### [module uglifyjs.AST_Symbol](#apidoc.module.uglifyjs.AST_Symbol)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Symbol (props)](#apidoc.element.uglifyjs.AST_Symbol.AST_Symbol)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Symbol.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Symbol.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>documentation

#### [module uglifyjs.AST_Symbol.SUBCLASSES](#apidoc.module.uglifyjs.AST_Symbol.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.4)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.5)

#### [module uglifyjs.AST_Symbol.prototype](#apidoc.module.uglifyjs.AST_Symbol.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Symbol.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Symbol.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Symbol.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>definition ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.definition)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>global ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.global)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>undeclared ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.undeclared)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>unmangleable (options)](#apidoc.element.uglifyjs.AST_Symbol.prototype.unmangleable)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>unreferenced ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.unreferenced)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolAccessor](#apidoc.module.uglifyjs.AST_SymbolAccessor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolAccessor (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor.AST_SymbolAccessor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolAccessor.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>documentation

#### [module uglifyjs.AST_SymbolAccessor.prototype](#apidoc.module.uglifyjs.AST_SymbolAccessor.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.prototype.</span>unmangleable ()](#apidoc.element.uglifyjs.AST_SymbolAccessor.prototype.unmangleable)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolCatch](#apidoc.module.uglifyjs.AST_SymbolCatch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolCatch (props)](#apidoc.element.uglifyjs.AST_SymbolCatch.AST_SymbolCatch)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolCatch.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolCatch.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>documentation

#### [module uglifyjs.AST_SymbolCatch.prototype](#apidoc.module.uglifyjs.AST_SymbolCatch.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolCatch.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolConst](#apidoc.module.uglifyjs.AST_SymbolConst)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolConst (props)](#apidoc.element.uglifyjs.AST_SymbolConst.AST_SymbolConst)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolConst.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolConst.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>documentation

#### [module uglifyjs.AST_SymbolConst.prototype](#apidoc.module.uglifyjs.AST_SymbolConst.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolConst.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolDeclaration](#apidoc.module.uglifyjs.AST_SymbolDeclaration)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.AST_SymbolDeclaration)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>documentation

#### [module uglifyjs.AST_SymbolDeclaration.SUBCLASSES](#apidoc.module.uglifyjs.AST_SymbolDeclaration.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.1)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.2)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.3)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.4)

#### [module uglifyjs.AST_SymbolDeclaration.prototype](#apidoc.module.uglifyjs.AST_SymbolDeclaration.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolDefun](#apidoc.module.uglifyjs.AST_SymbolDefun)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDefun (props)](#apidoc.element.uglifyjs.AST_SymbolDefun.AST_SymbolDefun)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolDefun.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolDefun.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>documentation

#### [module uglifyjs.AST_SymbolDefun.prototype](#apidoc.module.uglifyjs.AST_SymbolDefun.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolDefun.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolFunarg](#apidoc.module.uglifyjs.AST_SymbolFunarg)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolFunarg (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg.AST_SymbolFunarg)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolFunarg.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>documentation

#### [module uglifyjs.AST_SymbolFunarg.prototype](#apidoc.module.uglifyjs.AST_SymbolFunarg.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolLambda](#apidoc.module.uglifyjs.AST_SymbolLambda)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolLambda (props)](#apidoc.element.uglifyjs.AST_SymbolLambda.AST_SymbolLambda)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolLambda.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolLambda.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>documentation

#### [module uglifyjs.AST_SymbolLambda.prototype](#apidoc.module.uglifyjs.AST_SymbolLambda.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolLambda.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolRef](#apidoc.module.uglifyjs.AST_SymbolRef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolRef (props)](#apidoc.element.uglifyjs.AST_SymbolRef.AST_SymbolRef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolRef.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolRef.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>documentation

#### [module uglifyjs.AST_SymbolRef.prototype](#apidoc.module.uglifyjs.AST_SymbolRef.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>reference ()](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.reference)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>TYPE

#### [module uglifyjs.AST_SymbolVar](#apidoc.module.uglifyjs.AST_SymbolVar)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolVar (props)](#apidoc.element.uglifyjs.AST_SymbolVar.AST_SymbolVar)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolVar.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolVar.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>documentation

#### [module uglifyjs.AST_SymbolVar.SUBCLASSES](#apidoc.module.uglifyjs.AST_SymbolVar.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_SymbolVar.SUBCLASSES.0)

#### [module uglifyjs.AST_SymbolVar.prototype](#apidoc.module.uglifyjs.AST_SymbolVar.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolVar.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.prototype.</span>TYPE

#### [module uglifyjs.AST_This](#apidoc.module.uglifyjs.AST_This)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_This (props)](#apidoc.element.uglifyjs.AST_This.AST_This)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>BASE (props)](#apidoc.element.uglifyjs.AST_This.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_This.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>documentation

#### [module uglifyjs.AST_This.prototype](#apidoc.module.uglifyjs.AST_This.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_This.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_This.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_This.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_This.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>TYPE

#### [module uglifyjs.AST_Throw](#apidoc.module.uglifyjs.AST_Throw)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Throw (props)](#apidoc.element.uglifyjs.AST_Throw.AST_Throw)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Throw.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Throw.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>documentation

#### [module uglifyjs.AST_Throw.prototype](#apidoc.module.uglifyjs.AST_Throw.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Throw.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Throw.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Throw.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>TYPE

#### [module uglifyjs.AST_Token](#apidoc.module.uglifyjs.AST_Token)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Token (props)](#apidoc.element.uglifyjs.AST_Token.AST_Token)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Token.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Token.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Token.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Token.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Token.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Token.</span>TYPE

#### [module uglifyjs.AST_Token.prototype](#apidoc.module.uglifyjs.AST_Token.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Token.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Token.prototype.CTOR)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Token.prototype.</span>TYPE

#### [module uglifyjs.AST_Toplevel](#apidoc.module.uglifyjs.AST_Toplevel)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Toplevel (props)](#apidoc.element.uglifyjs.AST_Toplevel.AST_Toplevel)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Toplevel.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Toplevel.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>documentation

#### [module uglifyjs.AST_Toplevel.prototype](#apidoc.module.uglifyjs.AST_Toplevel.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Toplevel.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>_default_mangler_options (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype._default_mangler_options)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>compute_char_frequency (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.compute_char_frequency)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>figure_out_scope (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.figure_out_scope)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>mangle_names (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.mangle_names)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>scope_warnings (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.scope_warnings)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Toplevel.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>wrap_commonjs (name, export_all)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.wrap_commonjs)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>wrap_enclose (arg_parameter_pairs)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.wrap_enclose)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>TYPE

#### [module uglifyjs.AST_True](#apidoc.module.uglifyjs.AST_True)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_True (props)](#apidoc.element.uglifyjs.AST_True.AST_True)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>BASE (props)](#apidoc.element.uglifyjs.AST_True.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_True.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>documentation

#### [module uglifyjs.AST_True.prototype](#apidoc.module.uglifyjs.AST_True.prototype)
1.  boolean <span class="apidocSignatureSpan">uglifyjs.AST_True.prototype.</span>value
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_True.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_True.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_True.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_True.prototype.is_boolean)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_True.prototype.</span>TYPE

#### [module uglifyjs.AST_Try](#apidoc.module.uglifyjs.AST_Try)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Try (props)](#apidoc.element.uglifyjs.AST_Try.AST_Try)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Try.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Try.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>documentation

#### [module uglifyjs.AST_Try.prototype](#apidoc.module.uglifyjs.AST_Try.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Try.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Try.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Try.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Try.prototype.add_source_map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Try.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Try.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Try.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>TYPE

#### [module uglifyjs.AST_Unary](#apidoc.module.uglifyjs.AST_Unary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Unary (props)](#apidoc.element.uglifyjs.AST_Unary.AST_Unary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Unary.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Unary.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>documentation

#### [module uglifyjs.AST_Unary.SUBCLASSES](#apidoc.module.uglifyjs.AST_Unary.SUBCLASSES)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Unary.SUBCLASSES.0)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Unary.SUBCLASSES.1)

#### [module uglifyjs.AST_Unary.prototype](#apidoc.module.uglifyjs.AST_Unary.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Unary.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Unary.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Unary.prototype.has_side_effects)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglifyjs.AST_Unary.prototype.lift_sequences)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Unary.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Unary.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Unary.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>TYPE

#### [module uglifyjs.AST_UnaryPostfix](#apidoc.module.uglifyjs.AST_UnaryPostfix)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPostfix (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix.AST_UnaryPostfix)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>BASE (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_UnaryPostfix.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>documentation

#### [module uglifyjs.AST_UnaryPostfix.prototype](#apidoc.module.uglifyjs.AST_UnaryPostfix.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_UnaryPostfix.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_UnaryPostfix.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>TYPE

#### [module uglifyjs.AST_UnaryPrefix](#apidoc.module.uglifyjs.AST_UnaryPrefix)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPrefix (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix.AST_UnaryPrefix)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>BASE (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_UnaryPrefix.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>documentation

#### [module uglifyjs.AST_UnaryPrefix.prototype](#apidoc.module.uglifyjs.AST_UnaryPrefix.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype._eval)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.is_boolean)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>is_string ()](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.is_string)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.negate)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>TYPE

#### [module uglifyjs.AST_Undefined](#apidoc.module.uglifyjs.AST_Undefined)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Undefined (props)](#apidoc.element.uglifyjs.AST_Undefined.AST_Undefined)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Undefined.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Undefined.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>documentation

#### [module uglifyjs.AST_Undefined.prototype](#apidoc.module.uglifyjs.AST_Undefined.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Undefined.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Undefined.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Undefined.prototype.needs_parens)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Undefined.prototype.optimize)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>TYPE

#### [module uglifyjs.AST_Var](#apidoc.module.uglifyjs.AST_Var)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Var (props)](#apidoc.element.uglifyjs.AST_Var.AST_Var)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Var.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Var.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>documentation

#### [module uglifyjs.AST_Var.prototype](#apidoc.module.uglifyjs.AST_Var.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Var.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Var.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_Var.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Var.prototype._codegen)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_Var.prototype.</span>TYPE

#### [module uglifyjs.AST_VarDef](#apidoc.module.uglifyjs.AST_VarDef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_VarDef (props)](#apidoc.element.uglifyjs.AST_VarDef.AST_VarDef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>BASE (props)](#apidoc.element.uglifyjs.AST_VarDef.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_VarDef.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>documentation

#### [module uglifyjs.AST_VarDef.prototype](#apidoc.module.uglifyjs.AST_VarDef.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_VarDef.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_VarDef.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_VarDef.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_VarDef.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_VarDef.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>TYPE

#### [module uglifyjs.AST_While](#apidoc.module.uglifyjs.AST_While)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_While (props)](#apidoc.element.uglifyjs.AST_While.AST_While)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>BASE (props)](#apidoc.element.uglifyjs.AST_While.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_While.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>SUBCLASSES
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>documentation

#### [module uglifyjs.AST_While.prototype](#apidoc.module.uglifyjs.AST_While.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_While.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_While.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_While.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_While.prototype.optimize)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_While.prototype.to_mozilla_ast)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>TYPE

#### [module uglifyjs.AST_With](#apidoc.module.uglifyjs.AST_With)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>AST_With (props)](#apidoc.element.uglifyjs.AST_With.AST_With)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>BASE (props)](#apidoc.element.uglifyjs.AST_With.BASE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_With.DEFMETHOD)
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>SELF_PROPS
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>SUBCLASSES
1.  object <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>propdoc
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>TYPE
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>documentation

#### [module uglifyjs.AST_With.prototype](#apidoc.module.uglifyjs.AST_With.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_With.prototype.CTOR)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_With.prototype._codegen)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_With.prototype._walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_With.prototype.to_mozilla_ast)
1.  [function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_With.prototype.transform)
1.  string <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>TYPE

#### [module uglifyjs.Buffer](#apidoc.module.uglifyjs.Buffer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.uglifyjs.Buffer.Buffer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>alloc (size, fill, encoding)](#apidoc.element.uglifyjs.Buffer.alloc)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>allocUnsafe (size)](#apidoc.element.uglifyjs.Buffer.allocUnsafe)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>allocUnsafeSlow (size)](#apidoc.element.uglifyjs.Buffer.allocUnsafeSlow)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>byteLength (string, encoding)](#apidoc.element.uglifyjs.Buffer.byteLength)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>compare (a, b)](#apidoc.element.uglifyjs.Buffer.compare)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>concat (list, length)](#apidoc.element.uglifyjs.Buffer.concat)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>from (value, encodingOrOffset, length)](#apidoc.element.uglifyjs.Buffer.from)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>isBuffer (b)](#apidoc.element.uglifyjs.Buffer.isBuffer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>isEncoding (encoding)](#apidoc.element.uglifyjs.Buffer.isEncoding)
1.  number <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>poolSize

#### [module uglifyjs.Buffer.prototype](#apidoc.module.uglifyjs.Buffer.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.uglifyjs.Buffer.prototype.asciiSlice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.uglifyjs.Buffer.prototype.asciiWrite)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>base64Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.base64Slice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>base64Write ()](#apidoc.element.uglifyjs.Buffer.prototype.base64Write)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.uglifyjs.Buffer.prototype.compare)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>copy ()](#apidoc.element.uglifyjs.Buffer.prototype.copy)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>equals (b)](#apidoc.element.uglifyjs.Buffer.prototype.equals)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.fill)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>hexSlice ()](#apidoc.element.uglifyjs.Buffer.prototype.hexSlice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>hexWrite ()](#apidoc.element.uglifyjs.Buffer.prototype.hexWrite)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.includes)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>inspect ()](#apidoc.element.uglifyjs.Buffer.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.latin1Slice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>latin1Write ()](#apidoc.element.uglifyjs.Buffer.prototype.latin1Write)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readDoubleBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readDoubleLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readFloatBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readFloatLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt16BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt16LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt32BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt32LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt8)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readIntBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readIntLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt16BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt16LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt32BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt32LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt8)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUIntBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUIntLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>slice (start, end)](#apidoc.element.uglifyjs.Buffer.prototype.slice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>swap16 ()](#apidoc.element.uglifyjs.Buffer.prototype.swap16)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>swap32 ()](#apidoc.element.uglifyjs.Buffer.prototype.swap32)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>swap64 ()](#apidoc.element.uglifyjs.Buffer.prototype.swap64)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>toJSON ()](#apidoc.element.uglifyjs.Buffer.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>toString ()](#apidoc.element.uglifyjs.Buffer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.ucs2Slice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.uglifyjs.Buffer.prototype.ucs2Write)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.utf8Slice)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>utf8Write ()](#apidoc.element.uglifyjs.Buffer.prototype.utf8Write)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.write)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeDoubleBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeDoubleLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeFloatBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeFloatLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt16BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt16LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt32BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt32LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt8)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeIntBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeIntLE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt16BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt16LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt32BE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt32LE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt8)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUIntBE)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUIntLE)

#### [module uglifyjs.Compressor](#apidoc.module.uglifyjs.Compressor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>Compressor (options, false_by_default)](#apidoc.element.uglifyjs.Compressor.Compressor)

#### [module uglifyjs.Compressor.prototype](#apidoc.module.uglifyjs.Compressor.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>before (node, descend, in_list)](#apidoc.element.uglifyjs.Compressor.prototype.before)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>option (key)](#apidoc.element.uglifyjs.Compressor.prototype.option)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>warn ()](#apidoc.element.uglifyjs.Compressor.prototype.warn)
1.  object <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>stack

#### [module uglifyjs.DefaultsError](#apidoc.module.uglifyjs.DefaultsError)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>DefaultsError (msg, defs)](#apidoc.element.uglifyjs.DefaultsError.DefaultsError)
1.  [function <span class="apidocSignatureSpan">uglifyjs.DefaultsError.</span>croak (msg, defs)](#apidoc.element.uglifyjs.DefaultsError.croak)

#### [module uglifyjs.DefaultsError.prototype](#apidoc.module.uglifyjs.DefaultsError.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.DefaultsError.prototype.</span>constructor (msg, defs)](#apidoc.element.uglifyjs.DefaultsError.prototype.constructor)

#### [module uglifyjs.Dictionary](#apidoc.module.uglifyjs.Dictionary)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>Dictionary ()](#apidoc.element.uglifyjs.Dictionary.Dictionary)

#### [module uglifyjs.Dictionary.prototype](#apidoc.module.uglifyjs.Dictionary.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>add (key, val)](#apidoc.element.uglifyjs.Dictionary.prototype.add)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>del (key)](#apidoc.element.uglifyjs.Dictionary.prototype.del)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>each (f)](#apidoc.element.uglifyjs.Dictionary.prototype.each)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>get (key)](#apidoc.element.uglifyjs.Dictionary.prototype.get)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>has (key)](#apidoc.element.uglifyjs.Dictionary.prototype.has)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>map (f)](#apidoc.element.uglifyjs.Dictionary.prototype.map)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>set (key, val)](#apidoc.element.uglifyjs.Dictionary.prototype.set)
1.  [function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>size ()](#apidoc.element.uglifyjs.Dictionary.prototype.size)

#### [module uglifyjs.JS_Parse_Error](#apidoc.module.uglifyjs.JS_Parse_Error)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglifyjs.JS_Parse_Error.JS_Parse_Error)

#### [module uglifyjs.JS_Parse_Error.prototype](#apidoc.module.uglifyjs.JS_Parse_Error.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.JS_Parse_Error.prototype.</span>toString ()](#apidoc.element.uglifyjs.JS_Parse_Error.prototype.toString)

#### [module uglifyjs.MAP](#apidoc.module.uglifyjs.MAP)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>MAP (a, f, backwards)](#apidoc.element.uglifyjs.MAP.MAP)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MAP.</span>at_top (val)](#apidoc.element.uglifyjs.MAP.at_top)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MAP.</span>last (val)](#apidoc.element.uglifyjs.MAP.last)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MAP.</span>splice (val)](#apidoc.element.uglifyjs.MAP.splice)
1.  object <span class="apidocSignatureSpan">uglifyjs.MAP.</span>skip

#### [module uglifyjs.MOZ_SourceMap](#apidoc.module.uglifyjs.MOZ_SourceMap)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapConsumer (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapGenerator (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceNode (aLine, aColumn, aSource, aChunks, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode)

#### [module uglifyjs.MOZ_SourceMap.SourceMapConsumer](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapConsumer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapConsumer (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.SourceMapConsumer)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.</span>fromSourceMap (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.fromSourceMap)
1.  number <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.</span>GENERATED_ORDER
1.  number <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.</span>ORIGINAL_ORDER

#### [module uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>_findMapping (aNeedle, aMappings, aLineName, aColumnName, aComparator)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype._findMapping)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>_parseMappings (aStr, aSourceRoot)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype._parseMappings)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>eachMapping (aCallback, aContext, aOrder)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.eachMapping)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>generatedPositionFor (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.generatedPositionFor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>originalPositionFor (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.originalPositionFor)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>sourceContentFor (aSource)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.sourceContentFor)
1.  number <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>_version
1.  object <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>__generatedMappings
1.  object <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>__originalMappings

#### [module uglifyjs.MOZ_SourceMap.SourceMapGenerator](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapGenerator)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapGenerator (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.SourceMapGenerator)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.</span>fromSourceMap (aSourceMapConsumer)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.fromSourceMap)

#### [module uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_generateSourcesContent (aSources, aSourceRoot)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._generateSourcesContent)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_serializeMappings ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._serializeMappings)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_validateMapping (aGenerated, aOriginal, aSource, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._validateMapping)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>addMapping (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.addMapping)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>applySourceMap (aSourceMapConsumer, aSourceFile, aSourceMapPath)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.applySourceMap)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>setSourceContent (aSourceFile, aSourceContent)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.setSourceContent)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>toJSON ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>toString ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.toString)
1.  number <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_version

#### [module uglifyjs.MOZ_SourceMap.SourceNode](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceNode)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceNode (aLine, aColumn, aSource, aChunks, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.SourceNode)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.</span>fromStringWithSourceMap (aGeneratedCode, aSourceMapConsumer)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.fromStringWithSourceMap)

#### [module uglifyjs.MOZ_SourceMap.SourceNode.prototype](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceNode.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>add (aChunk)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.add)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>join (aSep)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.join)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>prepend (aChunk)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.prepend)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>replaceRight (aPattern, aReplacement)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.replaceRight)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>setSourceContent (aSourceFile, aSourceContent)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.setSourceContent)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>toString ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.toString)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>toStringWithSourceMap (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.toStringWithSourceMap)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>walk (aFn)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.walk)
1.  [function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>walkSourceContents (aFn)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.walkSourceContents)

#### [module uglifyjs.SymbolDef](#apidoc.module.uglifyjs.SymbolDef)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglifyjs.SymbolDef.SymbolDef)

#### [module uglifyjs.SymbolDef.prototype](#apidoc.module.uglifyjs.SymbolDef.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.SymbolDef.prototype.</span>mangle (options)](#apidoc.element.uglifyjs.SymbolDef.prototype.mangle)
1.  [function <span class="apidocSignatureSpan">uglifyjs.SymbolDef.prototype.</span>unmangleable (options)](#apidoc.element.uglifyjs.SymbolDef.prototype.unmangleable)

#### [module uglifyjs.TreeWalker](#apidoc.module.uglifyjs.TreeWalker)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>TreeWalker (callback)](#apidoc.element.uglifyjs.TreeWalker.TreeWalker)

#### [module uglifyjs.TreeWalker.prototype](#apidoc.module.uglifyjs.TreeWalker.prototype)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>_visit (node, descend)](#apidoc.element.uglifyjs.TreeWalker.prototype._visit)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>find_parent (type)](#apidoc.element.uglifyjs.TreeWalker.prototype.find_parent)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>has_directive (type)](#apidoc.element.uglifyjs.TreeWalker.prototype.has_directive)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>in_boolean_context ()](#apidoc.element.uglifyjs.TreeWalker.prototype.in_boolean_context)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>loopcontrol_target (label)](#apidoc.element.uglifyjs.TreeWalker.prototype.loopcontrol_target)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>parent (n)](#apidoc.element.uglifyjs.TreeWalker.prototype.parent)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>pop ()](#apidoc.element.uglifyjs.TreeWalker.prototype.pop)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>push (node)](#apidoc.element.uglifyjs.TreeWalker.prototype.push)
1.  [function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>self ()](#apidoc.element.uglifyjs.TreeWalker.prototype.self)

#### [module uglifyjs.base54](#apidoc.module.uglifyjs.base54)
1.  [function <span class="apidocSignatureSpan">uglifyjs.</span>base54 (num)](#apidoc.element.uglifyjs.base54.base54)
1.  [function <span class="apidocSignatureSpan">uglifyjs.base54.</span>consider (str)](#apidoc.element.uglifyjs.base54.consider)
1.  [function <span class="apidocSignatureSpan">uglifyjs.base54.</span>freq ()](#apidoc.element.uglifyjs.base54.freq)
1.  [function <span class="apidocSignatureSpan">uglifyjs.base54.</span>get ()](#apidoc.element.uglifyjs.base54.get)
1.  [function <span class="apidocSignatureSpan">uglifyjs.base54.</span>reset ()](#apidoc.element.uglifyjs.base54.reset)
1.  [function <span class="apidocSignatureSpan">uglifyjs.base54.</span>sort ()](#apidoc.element.uglifyjs.base54.sort)



# <a name="apidoc.module.uglifyjs"></a>[module uglifyjs](#apidoc.module.uglifyjs)

#### <a name="apidoc.element.uglifyjs.ASSIGNMENT"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>ASSIGNMENT (str )](#apidoc.element.uglifyjs.ASSIGNMENT)
- description and source-code
```javascript
function anonymous(str ) {
switch(str.length){case 2:switch(str){case "+=":case "-=":case "/=":case "*=":case "%=":case "|=":case "^=":case "&=":return true
}return false;case 3:switch(str){case ">>=":case "<<=":return true}return false;case 1:return str === "=";case 4:return str === ">>>=";}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Accessor"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Accessor (props)](#apidoc.element.uglifyjs.AST_Accessor)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Array"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Array (props)](#apidoc.element.uglifyjs.AST_Array)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Assign (props)](#apidoc.element.uglifyjs.AST_Assign)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Atom (props)](#apidoc.element.uglifyjs.AST_Atom)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Binary (props)](#apidoc.element.uglifyjs.AST_Binary)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Block (props)](#apidoc.element.uglifyjs.AST_Block)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_BlockStatement (props)](#apidoc.element.uglifyjs.AST_BlockStatement)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Boolean (props)](#apidoc.element.uglifyjs.AST_Boolean)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Break"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Break (props)](#apidoc.element.uglifyjs.AST_Break)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Call (props)](#apidoc.element.uglifyjs.AST_Call)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Case"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Case (props)](#apidoc.element.uglifyjs.AST_Case)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Catch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Catch (props)](#apidoc.element.uglifyjs.AST_Catch)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Conditional (props)](#apidoc.element.uglifyjs.AST_Conditional)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Const"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Const (props)](#apidoc.element.uglifyjs.AST_Const)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Constant (props)](#apidoc.element.uglifyjs.AST_Constant)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Continue"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Continue (props)](#apidoc.element.uglifyjs.AST_Continue)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_DWLoop"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_DWLoop (props)](#apidoc.element.uglifyjs.AST_DWLoop)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Debugger (props)](#apidoc.element.uglifyjs.AST_Debugger)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Default"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Default (props)](#apidoc.element.uglifyjs.AST_Default)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Definitions (props)](#apidoc.element.uglifyjs.AST_Definitions)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Defun"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Defun (props)](#apidoc.element.uglifyjs.AST_Defun)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Directive"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Directive (props)](#apidoc.element.uglifyjs.AST_Directive)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Do"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Do (props)](#apidoc.element.uglifyjs.AST_Do)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Dot (props)](#apidoc.element.uglifyjs.AST_Dot)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_EmptyStatement (props)](#apidoc.element.uglifyjs.AST_EmptyStatement)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Exit"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Exit (props)](#apidoc.element.uglifyjs.AST_Exit)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_False"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_False (props)](#apidoc.element.uglifyjs.AST_False)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Finally"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Finally (props)](#apidoc.element.uglifyjs.AST_Finally)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_For"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_For (props)](#apidoc.element.uglifyjs.AST_For)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ForIn (props)](#apidoc.element.uglifyjs.AST_ForIn)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Function (props)](#apidoc.element.uglifyjs.AST_Function)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Hole"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Hole (props)](#apidoc.element.uglifyjs.AST_Hole)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_If"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_If (props)](#apidoc.element.uglifyjs.AST_If)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Infinity"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Infinity (props)](#apidoc.element.uglifyjs.AST_Infinity)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_IterationStatement (props)](#apidoc.element.uglifyjs.AST_IterationStatement)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Jump"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Jump (props)](#apidoc.element.uglifyjs.AST_Jump)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Label"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Label (props)](#apidoc.element.uglifyjs.AST_Label)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabelRef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabelRef (props)](#apidoc.element.uglifyjs.AST_LabelRef)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabeledStatement (props)](#apidoc.element.uglifyjs.AST_LabeledStatement)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Lambda (props)](#apidoc.element.uglifyjs.AST_Lambda)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LoopControl (props)](#apidoc.element.uglifyjs.AST_LoopControl)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_NaN"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_NaN (props)](#apidoc.element.uglifyjs.AST_NaN)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_New (props)](#apidoc.element.uglifyjs.AST_New)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Node (props)](#apidoc.element.uglifyjs.AST_Node)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Null"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Null (props)](#apidoc.element.uglifyjs.AST_Null)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Number"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Number (props)](#apidoc.element.uglifyjs.AST_Number)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Object (props)](#apidoc.element.uglifyjs.AST_Object)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectGetter"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectGetter (props)](#apidoc.element.uglifyjs.AST_ObjectGetter)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectKeyVal"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectProperty (props)](#apidoc.element.uglifyjs.AST_ObjectProperty)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectSetter"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectSetter (props)](#apidoc.element.uglifyjs.AST_ObjectSetter)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_PropAccess (props)](#apidoc.element.uglifyjs.AST_PropAccess)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_RegExp"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_RegExp (props)](#apidoc.element.uglifyjs.AST_RegExp)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Return"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Return (props)](#apidoc.element.uglifyjs.AST_Return)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Scope (props)](#apidoc.element.uglifyjs.AST_Scope)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Seq (props)](#apidoc.element.uglifyjs.AST_Seq)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SimpleStatement (props)](#apidoc.element.uglifyjs.AST_SimpleStatement)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Statement (props)](#apidoc.element.uglifyjs.AST_Statement)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_StatementWithBody (props)](#apidoc.element.uglifyjs.AST_StatementWithBody)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_String"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_String (props)](#apidoc.element.uglifyjs.AST_String)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Sub"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Sub (props)](#apidoc.element.uglifyjs.AST_Sub)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Switch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Switch (props)](#apidoc.element.uglifyjs.AST_Switch)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SwitchBranch (props)](#apidoc.element.uglifyjs.AST_SwitchBranch)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Symbol (props)](#apidoc.element.uglifyjs.AST_Symbol)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolAccessor"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolAccessor (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolCatch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolCatch (props)](#apidoc.element.uglifyjs.AST_SymbolCatch)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolConst"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolConst (props)](#apidoc.element.uglifyjs.AST_SymbolConst)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDefun"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDefun (props)](#apidoc.element.uglifyjs.AST_SymbolDefun)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolFunarg"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolFunarg (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolLambda"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolLambda (props)](#apidoc.element.uglifyjs.AST_SymbolLambda)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolRef (props)](#apidoc.element.uglifyjs.AST_SymbolRef)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolVar"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolVar (props)](#apidoc.element.uglifyjs.AST_SymbolVar)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_This"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_This (props)](#apidoc.element.uglifyjs.AST_This)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Throw"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Throw (props)](#apidoc.element.uglifyjs.AST_Throw)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Token"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Token (props)](#apidoc.element.uglifyjs.AST_Token)
- description and source-code
```javascript
function AST_Token(props){ if (props) { this.file = props.file;this.comments_before = props.comments_before;this.nlb = props.nlb
;this.endpos = props.endpos;this.endcol = props.endcol;this.endline = props.endline;this.pos = props.pos;this.col = props.col;this
.line = props.line;this.value = props.value;this.type = props.type;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Toplevel (props)](#apidoc.element.uglifyjs.AST_Toplevel)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_True"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_True (props)](#apidoc.element.uglifyjs.AST_True)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Try"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Try (props)](#apidoc.element.uglifyjs.AST_Try)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Unary (props)](#apidoc.element.uglifyjs.AST_Unary)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPostfix (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPrefix (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Undefined"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Undefined (props)](#apidoc.element.uglifyjs.AST_Undefined)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Var"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Var (props)](#apidoc.element.uglifyjs.AST_Var)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_VarDef (props)](#apidoc.element.uglifyjs.AST_VarDef)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_While"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_While (props)](#apidoc.element.uglifyjs.AST_While)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_With"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_With (props)](#apidoc.element.uglifyjs.AST_With)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.uglifyjs.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Compressor"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>Compressor (options, false_by_default)](#apidoc.element.uglifyjs.Compressor)
- description and source-code
```javascript
function Compressor(options, false_by_default) {
    if (!(this instanceof Compressor))
        return new Compressor(options, false_by_default);
    TreeTransformer.call(this, this.before, this.after);
    this.options = defaults(options, {
        sequences     : !false_by_default,
        properties    : !false_by_default,
        dead_code     : !false_by_default,
        drop_debugger : !false_by_default,
        unsafe        : false,
        unsafe_comps  : false,
        conditionals  : !false_by_default,
        comparisons   : !false_by_default,
        evaluate      : !false_by_default,
        booleans      : !false_by_default,
        loops         : !false_by_default,
        unused        : !false_by_default,
        hoist_funs    : !false_by_default,
        keep_fargs    : false,
        keep_fnames   : false,
        hoist_vars    : false,
        if_return     : !false_by_default,
        join_vars     : !false_by_default,
        cascade       : !false_by_default,
        side_effects  : !false_by_default,
        pure_getters  : false,
        pure_funcs    : null,
        negate_iife   : !false_by_default,
        screw_ie8     : false,
        drop_console  : false,
        angular       : false,

        warnings      : true,
        global_defs   : {}
    }, true);
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```

#### <a name="apidoc.element.uglifyjs.DEFNODE"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>DEFNODE (type, props, methods, base)](#apidoc.element.uglifyjs.DEFNODE)
- description and source-code
```javascript
function DEFNODE(type, props, methods, base) {
    if (arguments.length < 4) base = AST_Node;
    if (!props) props = [];
    else props = props.split(/\s+/);
    var self_props = props;
    if (base && base.PROPS)
        props = props.concat(base.PROPS);
    var code = "return function AST_" + type + "(props){ if (props) { ";
    for (var i = props.length; --i >= 0;) {
        code += "this." + props[i] + " = props." + props[i] + ";";
    }
    var proto = base && new base;
    if (proto && proto.initialize || (methods && methods.initialize))
        code += "this.initialize();";
    code += "}}";
    var ctor = new Function(code)();
    if (proto) {
        ctor.prototype = proto;
        ctor.BASE = base;
    }
    if (base) base.SUBCLASSES.push(ctor);
    ctor.prototype.CTOR = ctor;
    ctor.PROPS = props || null;
    ctor.SELF_PROPS = self_props;
    ctor.SUBCLASSES = [];
    if (type) {
        ctor.prototype.TYPE = ctor.TYPE = type;
    }
    if (methods) for (i in methods) if (methods.hasOwnProperty(i)) {
        if (/^\$/.test(i)) {
            ctor[i.substr(1)] = methods[i];
        } else {
            ctor.prototype[i] = methods[i];
        }
    }
    ctor.DEFMETHOD = function(name, method) {
        this.prototype[name] = method;
    };
    return ctor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.DefaultsError"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>DefaultsError (msg, defs)](#apidoc.element.uglifyjs.DefaultsError)
- description and source-code
```javascript
function DefaultsError(msg, defs) {
    Error.call(this, msg);
    this.msg = msg;
    this.defs = defs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Dictionary"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>Dictionary ()](#apidoc.element.uglifyjs.Dictionary)
- description and source-code
```javascript
function Dictionary() {
    this._values = Object.create(null);
    this._size = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.JS_Parse_Error"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglifyjs.JS_Parse_Error)
- description and source-code
```javascript
function JS_Parse_Error(message, filename, line, col, pos) {
    this.message = message;
    this.filename = filename;
    this.line = line;
    this.col = col;
    this.pos = pos;
    this.stack = new Error().stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.KEYWORDS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>KEYWORDS (str )](#apidoc.element.uglifyjs.KEYWORDS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str.length){case 5:switch(str){case "break":case "catch":case "const":case "throw":case "while":return true}return false;
case 4:switch(str){case "case":case "else":case "void":case "with":return true}return false;case 6:switch(str){case "delete":case
 "return":case "switch":case "typeof":return true}return false;case 3:switch(str){case "for":case "new":case "try":case "var":return
 true}return false;case 8:switch(str){case "continue":case "debugger":case "function":return true}return false;case 2:switch(str
){case "do":case "if":case "in":return true}return false;case 7:switch(str){case "default":case "finally":return true}return false
;case 10:return str === "instanceof";}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.KEYWORDS_ATOM"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>KEYWORDS_ATOM (str )](#apidoc.element.uglifyjs.KEYWORDS_ATOM)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case "false":case "null":case "true":return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.KEYWORDS_BEFORE_EXPRESSION"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>KEYWORDS_BEFORE_EXPRESSION (str )](#apidoc.element.uglifyjs.KEYWORDS_BEFORE_EXPRESSION)
- description and source-code
```javascript
function anonymous(str ) {
switch(str.length){case 6:switch(str){case "return":case "delete":return true}return false;case 4:switch(str){case "else":case "
case":return true}return false;case 3:return str === "new";case 5:return str === "throw";}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MAP"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>MAP (a, f, backwards)](#apidoc.element.uglifyjs.MAP)
- description and source-code
```javascript
function MAP(a, f, backwards) {
    var ret = [], top = [], i;
    function doit() {
        var val = f(a[i], i);
        var is_last = val instanceof Last;
        if (is_last) val = val.v;
        if (val instanceof AtTop) {
            val = val.v;
            if (val instanceof Splice) {
                top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
            } else {
                top.push(val);
            }
        }
        else if (val !== skip) {
            if (val instanceof Splice) {
                ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
            } else {
                ret.push(val);
            }
        }
        return is_last;
    };
    if (a instanceof Array) {
        if (backwards) {
            for (i = a.length; --i >= 0;) if (doit()) break;
            ret.reverse();
            top.reverse();
        } else {
            for (i = 0; i < a.length; ++i) if (doit()) break;
        }
    }
    else {
        for (i in a) if (a.hasOwnProperty(i)) if (doit()) break;
    }
    return top.concat(ret);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceMapConsumer (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer)
- description and source-code
```javascript
function SourceMapConsumer(aSourceMap) {
  var sourceMap = aSourceMap;
  if (typeof aSourceMap === 'string') {
    sourceMap = JSON.parse(aSourceMap.replace(/^\)\]\}'/, ''));
  }

  var version = util.getArg(sourceMap, 'version');
  var sources = util.getArg(sourceMap, 'sources');
  // Sass 3.3 leaves out the 'names' array, so we deviate from the spec (which
  // requires the array) to play nice here.
  var names = util.getArg(sourceMap, 'names', []);
  var sourceRoot = util.getArg(sourceMap, 'sourceRoot', null);
  var sourcesContent = util.getArg(sourceMap, 'sourcesContent', null);
  var mappings = util.getArg(sourceMap, 'mappings');
  var file = util.getArg(sourceMap, 'file', null);

  // Once again, Sass deviates from the spec and supplies the version as a
  // string rather than a number, so we use loose equality checking here.
  if (version != this._version) {
    throw new Error('Unsupported version: ' + version);
  }

  // Pass 'true' below to allow duplicate names and sources. While source maps
  // are intended to be compressed and deduplicated, the TypeScript compiler
  // sometimes generates source maps with duplicates in them. See Github issue
  // #72 and bugzil.la/889492.
  this._names = ArraySet.fromArray(names, true);
  this._sources = ArraySet.fromArray(sources, true);

  this.sourceRoot = sourceRoot;
  this.sourcesContent = sourcesContent;
  this._mappings = mappings;
  this.file = file;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceMapGenerator (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator)
- description and source-code
```javascript
function SourceMapGenerator(aArgs) {
  if (!aArgs) {
    aArgs = {};
  }
  this._file = util.getArg(aArgs, 'file', null);
  this._sourceRoot = util.getArg(aArgs, 'sourceRoot', null);
  this._sources = new ArraySet();
  this._names = new ArraySet();
  this._mappings = [];
  this._sourcesContents = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>MOZ_SourceMap.SourceNode (aLine, aColumn, aSource, aChunks, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode)
- description and source-code
```javascript
function SourceNode(aLine, aColumn, aSource, aChunks, aName) {
  this.children = [];
  this.sourceContents = {};
  this.line = aLine === undefined ? null : aLine;
  this.column = aColumn === undefined ? null : aColumn;
  this.source = aSource === undefined ? null : aSource;
  this.name = aName === undefined ? null : aName;
  if (aChunks != null) this.add(aChunks);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.OPERATORS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>OPERATORS (str )](#apidoc.element.uglifyjs.OPERATORS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str.length){case 2:switch(str){case "in":case "++":case "--":case ">>":case "<<":case "<=":case ">=":case "==":case "!=":
case "+=":case "-=":case "/=":case "*=":case "%=":case "|=":case "^=":case "&=":case "&&":case "||":return true}return false;case
 1:switch(str){case "+":case "-":case "!":case "~":case "&":case "|":case "^":case "*":case "/":case "%":case "<":case ">":case "?":
case "=":return true}return false;case 3:switch(str){case "new":case ">>>":case "===":case "!==":case ">>=":case "<<=":return true
}return false;case 6:switch(str){case "typeof":case "delete":return true}return false;case 4:switch(str){case "void":case ">>>=":
return true}return false;case 10:return str === "instanceof";}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.OPERATOR_CHARS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>OPERATOR_CHARS (str )](#apidoc.element.uglifyjs.OPERATOR_CHARS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case "+":case "-":case "*":case "&":case "%":case "=":case "<":case ">":case "!":case "?":case "|":case "~":case "^":
return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.OutputStream"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>OutputStream (options)](#apidoc.element.uglifyjs.OutputStream)
- description and source-code
```javascript
function OutputStream(options) {

    options = defaults(options, {
        indent_start     : 0,
        indent_level     : 4,
        quote_keys       : false,
        space_colon      : true,
        ascii_only       : false,
        unescape_regexps : false,
        inline_script    : false,
        width            : 80,
        max_line_len     : 32000,
        beautify         : false,
        source_map       : null,
        bracketize       : false,
        semicolons       : true,
        comments         : false,
        preserve_line    : false,
        screw_ie8        : false,
        preamble         : null,
        quote_style      : 0
    }, true);

    var indentation = 0;
    var current_col = 0;
    var current_line = 1;
    var current_pos = 0;
    var OUTPUT = "";

    function to_ascii(str, identifier) {
        return str.replace(/[\u0080-\uffff]/g, function(ch) {
            var code = ch.charCodeAt(0).toString(16);
            if (code.length <= 2 && !identifier) {
                while (code.length < 2) code = "0" + code;
                return "\\x" + code;
            } else {
                while (code.length < 4) code = "0" + code;
                return "\\u" + code;
            }
        });
    };

    function make_string(str, quote) {
        var dq = 0, sq = 0;
        str = str.replace(/[\\\b\f\n\r\t\x22\x27\u2028\u2029\0\ufeff]/g, function(s){
            switch (s) {
              case "\\": return "\\\\";
              case "\b": return "\\b";
              case "\f": return "\\f";
              case "\n": return "\\n";
              case "\r": return "\\r";
              case "\u2028": return "\\u2028";
              case "\u2029": return "\\u2029";
              case '"': ++dq; return '"';
              case "'": ++sq; return "'";
              case "\0": return "\\x00";
              case "\ufeff": return "\\ufeff";
            }
            return s;
        });
        function quote_single() {
            return "'" + str.replace(/\x27/g, "\\'") + "'";
        }
        function quote_double() {
            return '"' + str.replace(/\x22/g, '\\"') + '"';
        }
        if (options.ascii_only) str = to_ascii(str);
        switch (options.quote_style) {
          case 1:
            return quote_single();
          case 2:
            return quote_double();
          case 3:
            return quote == "'" ? quote_single() : quote_double();
          default:
            return dq > sq ? quote_single() : quote_double();
        }
    };

    function encode_string(str, quote) {
        var ret = make_string(str, quote);
        if (options.inline_script)
            ret = ret.replace(/<\x2fscript([>\/\t\n\f\r ])/gi, "<\\/script$1");
        return ret;
    };

    function make_name(name) {
        name = name.toString();
        if (options.ascii_only)
            name = to_ascii(name, true);
        return name;
    };

    function make_indent(back) {
        return repeat_string(" ", options.indent_start + indentation - back * options.indent_level);
    };

<span class="apidocCodeCommentSpan">    /* -----[ beautification/minification ]----- */
</span>
    var might_need_space = false;
    var might_need_semicolon = false;
    var last = null;

    function last_char() {
        return last.charAt(last.length - 1);
    };

    function maybe_newline() {
        if (options.max_line_len && current_col > options.max_line_len)
            print("\n");
    };

    var requireSemicolonChars = makePredicate("( [ + * / - , .");

    function print(str) {
        str = String(str);
        var ch = str.charAt(0);
        if (might_need_semicolon) {
            if ((!ch || ";}".indexOf(ch) < 0) && !/[;]$/.test(last)) {
                if (options.semicolons || requireSemicolonChars(ch)) {
                    OUTPUT += ";";
                    current_col++;
                    current_pos++;
                } else {
                    OUTPUT += "\n";
                    current_pos++;
                    current_line++;
                    current_col = 0;
                }
                if (!options.beautify) ...
```
- example usage
```shell
...
'''

#### Generating output

AST nodes have a 'print' method that takes an output stream.  Essentially,
to generate code you do this:
'''javascript
var stream = UglifyJS.OutputStream(options);
compressed_ast.print(stream);
var code = stream.toString(); // this is your minified code
'''

or, for a shortcut you can do:
'''javascript
var code = compressed_ast.print_to_string(options);
...
```

#### <a name="apidoc.element.uglifyjs.PUNC_BEFORE_EXPRESSION"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>PUNC_BEFORE_EXPRESSION (str )](#apidoc.element.uglifyjs.PUNC_BEFORE_EXPRESSION)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case "[":case "{":case "(":case ",":case ".":case ";":case ":":return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.PUNC_CHARS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>PUNC_CHARS (str )](#apidoc.element.uglifyjs.PUNC_CHARS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case "[":case "]":case "{":case "}":case "(":case ")":case ",":case ";":case ":":return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.REGEXP_MODIFIERS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>REGEXP_MODIFIERS (str )](#apidoc.element.uglifyjs.REGEXP_MODIFIERS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case "g":case "m":case "s":case "i":case "y":return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.RESERVED_WORDS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>RESERVED_WORDS (str )](#apidoc.element.uglifyjs.RESERVED_WORDS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str.length){case 4:switch(str){case "byte":case "char":case "enum":case "goto":case "long":case "this":case "null":case "
true":case "case":case "else":case "void":case "with":return true}return false;case 5:switch(str){case "class":case "final":case
 "float":case "short":case "super":case "yield":case "false":case "break":case "catch":case "const":case "throw":case "while":return
 true}return false;case 6:switch(str){case "double":case "export":case "import":case "native":case "public":case "static":case "
throws":case "delete":case "return":case "switch":case "typeof":return true}return false;case 7:switch(str){case "boolean":case "
extends":case "package":case "private":case "default":case "finally":return true}return false;case 8:switch(str){case "abstract":
case "volatile":case "continue":case "debugger":case "function":return true}return false;case 3:switch(str){case "int":case "for
":case "new":case "try":case "var":return true}return false;case 9:switch(str){case "interface":case "protected":case "transient
":return true}return false;case 2:switch(str){case "do":case "if":case "in":return true}return false;case 10:switch(str){case "implements
":case "instanceof":return true}return false;case 12:return str === "synchronized";}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.SourceMap"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>SourceMap (options)](#apidoc.element.uglifyjs.SourceMap)
- description and source-code
```javascript
function SourceMap(options) {
    options = defaults(options, {
        file : null,
        root : null,
        orig : null,

        orig_line_diff : 0,
        dest_line_diff : 0,
    });
    var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
    var generator;
    if (orig_map) {
      generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
    } else {
        generator = new MOZ_SourceMap.SourceMapGenerator({
            file       : options.file,
            sourceRoot : options.root
        });
    }
    function add(source, gen_line, gen_col, orig_line, orig_col, name) {
        if (orig_map) {
            var info = orig_map.originalPositionFor({
                line: orig_line,
                column: orig_col
            });
            if (info.source === null) {
                return;
            }
            source = info.source;
            orig_line = info.line;
            orig_col = info.column;
            name = info.name || name;
        }
        generator.addMapping({
            generated : { line: gen_line + options.dest_line_diff, column: gen_col },
            original  : { line: orig_line + options.orig_line_diff, column: orig_col },
            source    : source,
            name      : name
        });
    }
    return {
        add        : add,
        get        : function() { return generator },
        toString   : function() { return JSON.stringify(generator.toJSON()); }
    };
}
```
- example usage
```shell
...

You need to pass the 'source_map' argument when calling 'print'.  It needs
to be a 'SourceMap' object (which is a thin wrapper on top of the
[source-map][source-map] library).

Example:
'''javascript
var source_map = UglifyJS.SourceMap(source_map_options);
var stream = UglifyJS.OutputStream({
	...
	source_map: source_map
});
compressed_ast.print(stream);

var code = stream.toString();
...
```

#### <a name="apidoc.element.uglifyjs.SymbolDef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglifyjs.SymbolDef)
- description and source-code
```javascript
function SymbolDef(scope, index, orig) {
    this.name = orig.name;
    this.orig = [ orig ];
    this.scope = scope;
    this.references = [];
    this.global = false;
    this.mangled_name = null;
    this.undeclared = false;
    this.constant = false;
    this.index = index;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.TreeTransformer"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>TreeTransformer (before, after)](#apidoc.element.uglifyjs.TreeTransformer)
- description and source-code
```javascript
function TreeTransformer(before, after) {
    TreeWalker.call(this);
    this.before = before;
    this.after = after;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.TreeWalker"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>TreeWalker (callback)](#apidoc.element.uglifyjs.TreeWalker)
- description and source-code
```javascript
function TreeWalker(callback) {
    this.visit = callback;
    this.stack = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.UNARY_POSTFIX"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>UNARY_POSTFIX (str )](#apidoc.element.uglifyjs.UNARY_POSTFIX)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case "--":case "++":return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.UNARY_PREFIX"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>UNARY_PREFIX (str )](#apidoc.element.uglifyjs.UNARY_PREFIX)
- description and source-code
```javascript
function anonymous(str ) {
switch(str.length){case 1:switch(str){case "!":case "~":case "-":case "+":return true}return false;case 6:switch(str){case "typeof
":case "delete":return true}return false;case 2:switch(str){case "--":case "++":return true}return false;case 4:return str === "
void";}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.WHITESPACE_CHARS"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>WHITESPACE_CHARS (str )](#apidoc.element.uglifyjs.WHITESPACE_CHARS)
- description and source-code
```javascript
function anonymous(str ) {
switch(str){case " ":case " ":case "\n":case "\r":case "\t":case "\f":case "\u000b":case "​":case "᠎":case " ":case " ":case " ":
case " ":case " ":case " ":case " ":case " ":case " ":case " ":case " ":case " ":case " ":case "　":return true}return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.all"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>all (array, predicate)](#apidoc.element.uglifyjs.all)
- description and source-code
```javascript
function all(array, predicate) {
    for (var i = array.length; --i >= 0;)
        if (!predicate(array[i]))
            return false;
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.array_to_hash"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>array_to_hash (a)](#apidoc.element.uglifyjs.array_to_hash)
- description and source-code
```javascript
function array_to_hash(a) {
    var ret = Object.create(null);
    for (var i = 0; i < a.length; ++i)
        ret[a[i]] = true;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.base54"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>base54 (num)](#apidoc.element.uglifyjs.base54)
- description and source-code
```javascript
function base54(num) {
    var ret = "", base = 54;
    num++;
    do {
        num--;
        ret += String.fromCharCode(chars[num % base]);
        num = Math.floor(num / base);
        base = 64;
    } while (num > 0);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.characters"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>characters (str)](#apidoc.element.uglifyjs.characters)
- description and source-code
```javascript
function characters(str) {
    return str.split("");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.defaults"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>defaults (args, defs, croak)](#apidoc.element.uglifyjs.defaults)
- description and source-code
```javascript
function defaults(args, defs, croak) {
    if (args === true)
        args = {};
    var ret = args || {};
    if (croak) for (var i in ret) if (ret.hasOwnProperty(i) && !defs.hasOwnProperty(i))
        DefaultsError.croak("'" + i + "' is not a supported option", defs);
    for (var i in defs) if (defs.hasOwnProperty(i)) {
        ret[i] = (args && args.hasOwnProperty(i)) ? args[i] : defs[i];
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.describe_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>describe_ast ()](#apidoc.element.uglifyjs.describe_ast)
- description and source-code
```javascript
describe_ast = function () {
    var out = UglifyJS.OutputStream({ beautify: true });
    function doitem(ctor) {
        out.print("AST_" + ctor.TYPE);
        var props = ctor.SELF_PROPS.filter(function(prop){
            return !/^\$/.test(prop);
        });
        if (props.length > 0) {
            out.space();
            out.with_parens(function(){
                props.forEach(function(prop, i){
                    if (i) out.space();
                    out.print(prop);
                });
            });
        }
        if (ctor.documentation) {
            out.space();
            out.print_string(ctor.documentation);
        }
        if (ctor.SUBCLASSES.length > 0) {
            out.space();
            out.with_block(function(){
                ctor.SUBCLASSES.forEach(function(ctor, i){
                    out.indent();
                    doitem(ctor);
                    out.newline();
                });
            });
        }
    };
    doitem(UglifyJS.AST_Node);
    return out + "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.find_if"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>find_if (func, array)](#apidoc.element.uglifyjs.find_if)
- description and source-code
```javascript
function find_if(func, array) {
    for (var i = 0, n = array.length; i < n; ++i) {
        if (func(array[i]))
            return array[i];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_alphanumeric_char"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_alphanumeric_char (code)](#apidoc.element.uglifyjs.is_alphanumeric_char)
- description and source-code
```javascript
function is_alphanumeric_char(code) {
    return is_digit(code) || is_letter(code);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_digit"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_digit (code)](#apidoc.element.uglifyjs.is_digit)
- description and source-code
```javascript
function is_digit(code) {
    return code >= 48 && code <= 57;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_identifier"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier (name)](#apidoc.element.uglifyjs.is_identifier)
- description and source-code
```javascript
function is_identifier(name) {
    return !RESERVED_WORDS(name) && /^[a-z_$][a-z0-9_$]*$/i.test(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_identifier_char"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier_char (ch)](#apidoc.element.uglifyjs.is_identifier_char)
- description and source-code
```javascript
function is_identifier_char(ch) {
    var code = ch.charCodeAt(0);
    return is_identifier_start(code)
        || is_digit(code)
        || code == 8204 // \u200c: zero-width non-joiner <ZWNJ>
        || code == 8205 // \u200d: zero-width joiner <ZWJ> (in my ECMA-262 PDF, this is also 200c)
        || is_unicode_combining_mark(ch)
        || is_unicode_connector_punctuation(ch)
        || is_unicode_digit(code)
    ;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_identifier_start"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier_start (code)](#apidoc.element.uglifyjs.is_identifier_start)
- description and source-code
```javascript
function is_identifier_start(code) {
    return code == 36 || code == 95 || is_letter(code);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_identifier_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_identifier_string (str)](#apidoc.element.uglifyjs.is_identifier_string)
- description and source-code
```javascript
function is_identifier_string(str){
    return /^[a-z_$][a-z0-9_$]*$/i.test(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_letter"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_letter (code)](#apidoc.element.uglifyjs.is_letter)
- description and source-code
```javascript
function is_letter(code) {
    return (code >= 97 && code <= 122)
        || (code >= 65 && code <= 90)
        || (code >= 0xaa && UNICODE.letter.test(String.fromCharCode(code)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_token"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_token (token, type, val)](#apidoc.element.uglifyjs.is_token)
- description and source-code
```javascript
function is_token(token, type, val) {
    return token.type == type && (val == null || token.value == val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_unicode_combining_mark"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_unicode_combining_mark (ch)](#apidoc.element.uglifyjs.is_unicode_combining_mark)
- description and source-code
```javascript
function is_unicode_combining_mark(ch) {
    return UNICODE.non_spacing_mark.test(ch) || UNICODE.space_combining_mark.test(ch);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_unicode_connector_punctuation"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_unicode_connector_punctuation (ch)](#apidoc.element.uglifyjs.is_unicode_connector_punctuation)
- description and source-code
```javascript
function is_unicode_connector_punctuation(ch) {
    return UNICODE.connector_punctuation.test(ch);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.is_unicode_digit"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>is_unicode_digit (code)](#apidoc.element.uglifyjs.is_unicode_digit)
- description and source-code
```javascript
function is_unicode_digit(code) {
    return UNICODE.digit.test(String.fromCharCode(code));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.js_error"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>js_error (message, filename, line, col, pos)](#apidoc.element.uglifyjs.js_error)
- description and source-code
```javascript
function js_error(message, filename, line, col, pos) {
    throw new JS_Parse_Error(message, filename, line, col, pos);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.makePredicate"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>makePredicate (words)](#apidoc.element.uglifyjs.makePredicate)
- description and source-code
```javascript
function makePredicate(words) {
    if (!(words instanceof Array)) words = words.split(" ");
    var f = "", cats = [];
    out: for (var i = 0; i < words.length; ++i) {
        for (var j = 0; j < cats.length; ++j)
            if (cats[j][0].length == words[i].length) {
                cats[j].push(words[i]);
                continue out;
            }
        cats.push([words[i]]);
    }
    function compareTo(arr) {
        if (arr.length == 1) return f += "return str === " + JSON.stringify(arr[0]) + ";";
        f += "switch(str){";
        for (var i = 0; i < arr.length; ++i) f += "case " + JSON.stringify(arr[i]) + ":";
        f += "return true}return false;";
    }
    // When there are more than three length categories, an outer
    // switch first dispatches on the lengths, to save on comparisons.
    if (cats.length > 3) {
        cats.sort(function(a, b) {return b.length - a.length;});
        f += "switch(str.length){";
        for (var i = 0; i < cats.length; ++i) {
            var cat = cats[i];
            f += "case " + cat[0].length + ":";
            compareTo(cat);
        }
        f += "}";
        // Otherwise, simply generate a flat 'switch' statement.
    } else {
        compareTo(words);
    }
    return new Function("str", f);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.member"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>member (name, array)](#apidoc.element.uglifyjs.member)
- description and source-code
```javascript
function member(name, array) {
    for (var i = array.length; --i >= 0;)
        if (array[i] == name)
            return true;
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.merge"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>merge (obj, ext)](#apidoc.element.uglifyjs.merge)
- description and source-code
```javascript
function merge(obj, ext) {
    for (var i in ext) if (ext.hasOwnProperty(i)) {
        obj[i] = ext[i];
    }
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.mergeSort"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>mergeSort (array, cmp)](#apidoc.element.uglifyjs.mergeSort)
- description and source-code
```javascript
function mergeSort(array, cmp) {
    if (array.length < 2) return array.slice();
    function merge(a, b) {
        var r = [], ai = 0, bi = 0, i = 0;
        while (ai < a.length && bi < b.length) {
            cmp(a[ai], b[bi]) <= 0
                ? r[i++] = a[ai++]
                : r[i++] = b[bi++];
        }
        if (ai < a.length) r.push.apply(r, a.slice(ai));
        if (bi < b.length) r.push.apply(r, b.slice(bi));
        return r;
    };
    function _ms(a) {
        if (a.length <= 1)
            return a;
        var m = Math.floor(a.length / 2), left = a.slice(0, m), right = a.slice(m);
        left = _ms(left);
        right = _ms(right);
        return merge(left, right);
    };
    return _ms(array);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.minify"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>minify (files, options)](#apidoc.element.uglifyjs.minify)
- description and source-code
```javascript
minify = function (files, options) {
    options = UglifyJS.defaults(options, {
        spidermonkey : false,
        outSourceMap : null,
        sourceRoot   : null,
        inSourceMap  : null,
        fromString   : false,
        warnings     : false,
        mangle       : {},
        output       : null,
        compress     : {}
    });
    UglifyJS.base54.reset();

    // 1. parse
    var toplevel = null,
        sourcesContent = {};

    if (options.spidermonkey) {
        toplevel = UglifyJS.AST_Node.from_mozilla_ast(files);
    } else {
        if (typeof files == "string")
            files = [ files ];
        files.forEach(function(file){
            var code = options.fromString
                ? file
                : fs.readFileSync(file, "utf8");
            sourcesContent[file] = code;
            toplevel = UglifyJS.parse(code, {
                filename: options.fromString ? "?" : file,
                toplevel: toplevel
            });
        });
    }

    // 2. compress
    if (options.compress) {
        var compress = { warnings: options.warnings };
        UglifyJS.merge(compress, options.compress);
        toplevel.figure_out_scope();
        var sq = UglifyJS.Compressor(compress);
        toplevel = toplevel.transform(sq);
    }

    // 3. mangle
    if (options.mangle) {
        toplevel.figure_out_scope(options.mangle);
        toplevel.compute_char_frequency(options.mangle);
        toplevel.mangle_names(options.mangle);
    }

    // 4. output
    var inMap = options.inSourceMap;
    var output = {};
    if (typeof options.inSourceMap == "string") {
        inMap = fs.readFileSync(options.inSourceMap, "utf8");
    }
    if (options.outSourceMap) {
        output.source_map = UglifyJS.SourceMap({
            file: options.outSourceMap,
            orig: inMap,
            root: options.sourceRoot
        });
        if (options.sourceMapIncludeSources) {
            for (var file in sourcesContent) {
                if (sourcesContent.hasOwnProperty(file)) {
                    output.source_map.get().setSourceContent(file, sourcesContent[file]);
                }
            }
        }

    }
    if (options.output) {
        UglifyJS.merge(output, options.output);
    }
    var stream = UglifyJS.OutputStream(output);
    toplevel.print(stream);

    if(options.outSourceMap){
        stream += "\n//# sourceMappingURL=" + options.outSourceMap;
    }

    var source_map = output.source_map;
    if (source_map) {
        source_map = source_map + "";
    }

    return {
        code : stream + "",
        map  : source_map
    };
}
```
- example usage
```shell
...

### The simple way

There's a single toplevel function which combines all the steps.  If you
don't need additional customization, you might want to go with 'minify'.
Example:
'''javascript
var result = UglifyJS.minify("/path/to/file.js");
console.log(result.code); // minified output
// if you need to pass code instead of file name
var result = UglifyJS.minify("var b = function () {};", {fromString: true});
'''

You can also compress multiple files:
'''javascript
...
```

#### <a name="apidoc.element.uglifyjs.noop"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>noop ()](#apidoc.element.uglifyjs.noop)
- description and source-code
```javascript
function noop() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.parse"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>parse ($TEXT, options)](#apidoc.element.uglifyjs.parse)
- description and source-code
```javascript
function parse($TEXT, options) {

    options = defaults(options, {
        strict         : false,
        filename       : null,
        toplevel       : null,
        expression     : false,
        html5_comments : true,
        bare_returns   : false,
    });

    var S = {
        input         : (typeof $TEXT == "string"
                         ? tokenizer($TEXT, options.filename,
                                     options.html5_comments)
                         : $TEXT),
        token         : null,
        prev          : null,
        peeked        : null,
        in_function   : 0,
        in_directives : true,
        in_loop       : 0,
        labels        : []
    };

    S.token = next();

    function is(type, value) {
        return is_token(S.token, type, value);
    };

    function peek() { return S.peeked || (S.peeked = S.input()); };

    function next() {
        S.prev = S.token;
        if (S.peeked) {
            S.token = S.peeked;
            S.peeked = null;
        } else {
            S.token = S.input();
        }
        S.in_directives = S.in_directives && (
            S.token.type == "string" || is("punc", ";")
        );
        return S.token;
    };

    function prev() {
        return S.prev;
    };

    function croak(msg, line, col, pos) {
        var ctx = S.input.context();
        js_error(msg,
                 ctx.filename,
                 line != null ? line : ctx.tokline,
                 col != null ? col : ctx.tokcol,
                 pos != null ? pos : ctx.tokpos);
    };

    function token_error(token, msg) {
        croak(msg, token.line, token.col);
    };

    function unexpected(token) {
        if (token == null)
            token = S.token;
        token_error(token, "Unexpected token: " + token.type + " (" + token.value + ")");
    };

    function expect_token(type, val) {
        if (is(type, val)) {
            return next();
        }
        token_error(S.token, "Unexpected token " + S.token.type + " «" + S.token.value + "»" + ", expected " + type + " «" + val
 + "»");
    };

    function expect(punc) { return expect_token("punc", punc); };

    function can_insert_semicolon() {
        return !options.strict && (
            S.token.nlb || is("eof") || is("punc", "}")
        );
    };

    function semicolon() {
        if (is("punc", ";")) next();
        else if (!can_insert_semicolon()) unexpected();
    };

    function parenthesised() {
        expect("(");
        var exp = expression(true);
        expect(")");
        return exp;
    };

    function embed_tokens(parser) {
        return function() {
            var start = S.token;
            var expr = parser();
            var end = prev();
            expr.start = start;
            expr.end = end;
            return expr;
        };
    };

    function handle_regexp() {
        if (is("operator", "/") || is("operator", "/=")) {
            S.peeked = null;
            S.token = S.input(S.token.value.substr(1)); // force regexp
        }
    };

    var statement = embed_tokens(function() {
        var tmp;
        handle_regexp();
        switch (S.token.type) {
          case "string":
            var dir = S.in_directives, stat = simple_statement();
            // XXXv2: decide how to fix directives
            if (dir && stat.body instanceof AST_String && !is("punc", ",")) {
                return new AST_Directive({
                    start : stat.body.start,
                    end   : stat.body.end,
                    quote : stat.body.quote,
                    value : stat.body.value,
                });
            }
            return stat;
          case "num":
          case "regexp":
          case "operator":
          case "atom":
            return simple_statement();

          case "name":
            return is_token(peek(), "punc", ":")
                ? labeled_statement()
                : simple_statement();

          case "punc":
            switch (S.token.value) {
              case "{":
                return new AST_BlockStatement({ ...
```
- example usage
```shell
...
### The hard way

Following there's more detailed API info, in case the 'minify' function is
too simple for your needs.

#### The parser
'''javascript
var toplevel_ast = UglifyJS.parse(code, options);
'''

'options' is optional and if present it must be an object.  The following
properties are available:

- 'strict' — disable automatic semicolon insertion and support for trailing
comma in arrays and objects
...
```

#### <a name="apidoc.element.uglifyjs.parse_js_number"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>parse_js_number (num)](#apidoc.element.uglifyjs.parse_js_number)
- description and source-code
```javascript
function parse_js_number(num) {
    if (RE_HEX_NUMBER.test(num)) {
        return parseInt(num.substr(2), 16);
    } else if (RE_OCT_NUMBER.test(num)) {
        return parseInt(num.substr(1), 8);
    } else if (RE_DEC_NUMBER.test(num)) {
        return parseFloat(num);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.push_uniq"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>push_uniq (array, el)](#apidoc.element.uglifyjs.push_uniq)
- description and source-code
```javascript
function push_uniq(array, el) {
    if (array.indexOf(el) < 0)
        array.push(el);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.remove"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>remove (array, el)](#apidoc.element.uglifyjs.remove)
- description and source-code
```javascript
function remove(array, el) {
    for (var i = array.length; --i >= 0;) {
        if (array[i] === el) array.splice(i, 1);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.repeat_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>repeat_string (str, i)](#apidoc.element.uglifyjs.repeat_string)
- description and source-code
```javascript
function repeat_string(str, i) {
    if (i <= 0) return "";
    if (i == 1) return str;
    var d = repeat_string(str, i >> 1);
    d += d;
    if (i & 1) d += str;
    return d;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.set_difference"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>set_difference (a, b)](#apidoc.element.uglifyjs.set_difference)
- description and source-code
```javascript
function set_difference(a, b) {
    return a.filter(function(el){
        return b.indexOf(el) < 0;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.set_intersection"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>set_intersection (a, b)](#apidoc.element.uglifyjs.set_intersection)
- description and source-code
```javascript
function set_intersection(a, b) {
    return a.filter(function(el){
        return b.indexOf(el) >= 0;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.slice"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>slice (a, start)](#apidoc.element.uglifyjs.slice)
- description and source-code
```javascript
function slice(a, start) {
    return Array.prototype.slice.call(a, start || 0);
}
```
- example usage
```shell
...
        function doit() {
var val = f(a[i], i);
var is_last = val instanceof Last;
if (is_last) val = val.v;
if (val instanceof AtTop) {
    val = val.v;
    if (val instanceof Splice) {
        top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
    } else {
        top.push(val);
    }
}
else if (val !== skip) {
    if (val instanceof Splice) {
        ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
...
```

#### <a name="apidoc.element.uglifyjs.string_template"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>string_template (text, props)](#apidoc.element.uglifyjs.string_template)
- description and source-code
```javascript
function string_template(text, props) {
    return text.replace(/\{(.+?)\}/g, function(str, p){
        return props[p];
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.tokenizer"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>tokenizer ($TEXT, filename, html5_comments)](#apidoc.element.uglifyjs.tokenizer)
- description and source-code
```javascript
function tokenizer($TEXT, filename, html5_comments) {

    var S = {
        text            : $TEXT.replace(/\uFEFF/g, ''),
        filename        : filename,
        pos             : 0,
        tokpos          : 0,
        line            : 1,
        tokline         : 0,
        col             : 0,
        tokcol          : 0,
        newline_before  : false,
        regex_allowed   : false,
        comments_before : []
    };

    function peek() { return S.text.charAt(S.pos); };

    function next(signal_eof, in_string) {
        var ch = S.text.charAt(S.pos++);
        if (signal_eof && !ch)
            throw EX_EOF;
        if ("\r\n\u2028\u2029".indexOf(ch) >= 0) {
            S.newline_before = S.newline_before || !in_string;
            ++S.line;
            S.col = 0;
            if (!in_string && ch == "\r" && peek() == "\n") {
                // treat a \r\n sequence as a single \n
                ++S.pos;
                ch = "\n";
            }
        } else {
            ++S.col;
        }
        return ch;
    };

    function forward(i) {
        while (i-- > 0) next();
    };

    function looking_at(str) {
        return S.text.substr(S.pos, str.length) == str;
    };

    function find(what, signal_eof) {
        var pos = S.text.indexOf(what, S.pos);
        if (signal_eof && pos == -1) throw EX_EOF;
        return pos;
    };

    function start_token() {
        S.tokline = S.line;
        S.tokcol = S.col;
        S.tokpos = S.pos;
    };

    var prev_was_dot = false;
    function token(type, value, is_comment) {
        S.regex_allowed = ((type == "operator" && !UNARY_POSTFIX(value)) ||
                           (type == "keyword" && KEYWORDS_BEFORE_EXPRESSION(value)) ||
                           (type == "punc" && PUNC_BEFORE_EXPRESSION(value)));
        prev_was_dot = (type == "punc" && value == ".");
        var ret = {
            type    : type,
            value   : value,
            line    : S.tokline,
            col     : S.tokcol,
            pos     : S.tokpos,
            endline : S.line,
            endcol  : S.col,
            endpos  : S.pos,
            nlb     : S.newline_before,
            file    : filename
        };
        if (!is_comment) {
            ret.comments_before = S.comments_before;
            S.comments_before = [];
            // make note of any newlines in the comments that came before
            for (var i = 0, len = ret.comments_before.length; i < len; i++) {
                ret.nlb = ret.nlb || ret.comments_before[i].nlb;
            }
        }
        S.newline_before = false;
        return new AST_Token(ret);
    };

    function skip_whitespace() {
        while (WHITESPACE_CHARS(peek()))
            next();
    };

    function read_while(pred) {
        var ret = "", ch, i = 0;
        while ((ch = peek()) && pred(ch, i++))
            ret += next();
        return ret;
    };

    function parse_error(err) {
        js_error(err, filename, S.tokline, S.tokcol, S.tokpos);
    };

    function read_num(prefix) {
        var has_e = false, after_e = false, has_x = false, has_dot = prefix == ".";
        var num = read_while(function(ch, i){
            var code = ch.charCodeAt(0);
            switch (code) {
              case 120: case 88: // xX
                return has_x ? false : (has_x = true);
              case 101: case 69: // eE
                return has_x ? true : has_e ? false : (has_e = after_e = true);
              case 45: // -
                return after_e || (i == 0 && !prefix);
              case 43: // +
                return after_e;
              case (after_e = false, 46): // .
                return (!has_dot && !has_x && !has_e) ? (has_dot = true) : false;
            }
            return is_alphanumeric_char(code);
        });
        if (prefix) num = prefix + num;
        var valid = parse_js_number(num);
        if (!isNaN(valid)) {
            return token("num", valid);
        } else {
            parse_error("Invalid syntax: " + num);
        }
    };

    function read_escaped_char(in_string) { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.walk_body"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>walk_body (node, visitor)](#apidoc.element.uglifyjs.walk_body)
- description and source-code
```javascript
function walk_body(node, visitor) {
    if (node.body instanceof AST_Statement) {
        node.body._walk(visitor);
    }
    else node.body.forEach(function(stat){
        stat._walk(visitor);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Accessor"></a>[module uglifyjs.AST_Accessor](#apidoc.module.uglifyjs.AST_Accessor)

#### <a name="apidoc.element.uglifyjs.AST_Accessor.AST_Accessor"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Accessor (props)](#apidoc.element.uglifyjs.AST_Accessor.AST_Accessor)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Accessor.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Accessor.BASE)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Accessor.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Accessor.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Accessor.prototype"></a>[module uglifyjs.AST_Accessor.prototype](#apidoc.module.uglifyjs.AST_Accessor.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Accessor.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Accessor.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Accessor.prototype.CTOR)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_Array"></a>[module uglifyjs.AST_Array](#apidoc.module.uglifyjs.AST_Array)

#### <a name="apidoc.element.uglifyjs.AST_Array.AST_Array"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Array (props)](#apidoc.element.uglifyjs.AST_Array.AST_Array)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Array.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Array.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Array.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Array.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Array.prototype"></a>[module uglifyjs.AST_Array.prototype](#apidoc.module.uglifyjs.AST_Array.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Array.prototype.CTOR)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Array.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.with_square(function(){
        var a = self.elements, len = a.length;
        if (len > 0) output.space();
        a.forEach(function(exp, i){
            if (i) output.comma();
            exp.print(output);
            // If the final element is a hole, we need to make sure it
            // doesn't look like a trailing comma, by inserting an actual
            // trailing comma.
            if (i === len - 1 && exp instanceof AST_Hole)
              output.comma();
        });
        if (len > 0) output.space();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Array.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.elements.forEach(function(el){
            el._walk(visitor);
        });
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Array.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    for (var i = this.elements.length; --i >= 0;)
        if (this.elements[i].has_side_effects(compressor))
            return true;
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Array.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Array.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Array.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Array.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Array.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Assign"></a>[module uglifyjs.AST_Assign](#apidoc.module.uglifyjs.AST_Assign)

#### <a name="apidoc.element.uglifyjs.AST_Assign.AST_Assign"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Assign (props)](#apidoc.element.uglifyjs.AST_Assign.AST_Assign)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Assign.BASE)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Assign.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Assign.prototype"></a>[module uglifyjs.AST_Assign.prototype](#apidoc.module.uglifyjs.AST_Assign.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Assign.prototype.CTOR)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Assign.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return true }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Assign.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return this.operator == "=" && this.right.is_boolean();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Assign.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return (this.operator == "=" || this.operator == "+=") && this.right.is_string(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Assign.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    // !(a = false) → true
    if (p instanceof AST_Unary)
        return true;
    // 1 + (a = 2) + 3 → 6, side effect setting a = 2
    if (p instanceof AST_Binary && !(p instanceof AST_Assign))
        return true;
    // (a = func)() —or— new (a = Object)()
    if (p instanceof AST_Call && p.expression === this)
        return true;
    // (a = foo) ? bar : baz
    if (p instanceof AST_Conditional && p.condition === this)
        return true;
    // (a = foo)["prop"] —or— (a = foo).prop
    if (p instanceof AST_PropAccess && p.expression === this)
        return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Assign.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Assign.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Assign.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Assign.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Atom"></a>[module uglifyjs.AST_Atom](#apidoc.module.uglifyjs.AST_Atom)

#### <a name="apidoc.element.uglifyjs.AST_Atom.AST_Atom"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Atom (props)](#apidoc.element.uglifyjs.AST_Atom.AST_Atom)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Atom.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Atom.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Atom.SUBCLASSES"></a>[module uglifyjs.AST_Atom.SUBCLASSES](#apidoc.module.uglifyjs.AST_Atom.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.1)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.4)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Atom.SUBCLASSES.5)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Atom.prototype"></a>[module uglifyjs.AST_Atom.prototype](#apidoc.module.uglifyjs.AST_Atom.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Atom.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Atom.prototype.CTOR)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Atom.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Atom.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Atom.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Binary"></a>[module uglifyjs.AST_Binary](#apidoc.module.uglifyjs.AST_Binary)

#### <a name="apidoc.element.uglifyjs.AST_Binary.AST_Binary"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Binary (props)](#apidoc.element.uglifyjs.AST_Binary.AST_Binary)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Binary.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Binary.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Binary.SUBCLASSES"></a>[module uglifyjs.AST_Binary.SUBCLASSES](#apidoc.module.uglifyjs.AST_Binary.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Binary.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Binary.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Assign(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Binary.prototype"></a>[module uglifyjs.AST_Binary.prototype](#apidoc.module.uglifyjs.AST_Binary.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Binary.prototype.CTOR)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Binary.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.left.print(output);
    output.space();
    output.print(self.operator);
    if (self.operator == "<"
        && self.right instanceof AST_UnaryPrefix
        && self.right.operator == "!"
        && self.right.expression instanceof AST_UnaryPrefix
        && self.right.expression.operator == "--") {
        // space is mandatory to avoid outputting <!--
        // http://javascript.spec.whatwg.org/#comment-syntax
        output.print(" ");
    } else {
        // the space is optional depending on "beautify"
        output.space();
    }
    self.right.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>_eval (c)](#apidoc.element.uglifyjs.AST_Binary.prototype._eval)
- description and source-code
```javascript
_eval = function (c){
    var left = this.left, right = this.right;
    switch (this.operator) {
      case "&&"         : return ev(left, c) &&         ev(right, c);
      case "||"         : return ev(left, c) ||         ev(right, c);
      case "|"          : return ev(left, c) |          ev(right, c);
      case "&"          : return ev(left, c) &          ev(right, c);
      case "^"          : return ev(left, c) ^          ev(right, c);
      case "+"          : return ev(left, c) +          ev(right, c);
      case "*"          : return ev(left, c) *          ev(right, c);
      case "/"          : return ev(left, c) /          ev(right, c);
      case "%"          : return ev(left, c) %          ev(right, c);
      case "-"          : return ev(left, c) -          ev(right, c);
      case "<<"         : return ev(left, c) <<         ev(right, c);
      case ">>"         : return ev(left, c) >>         ev(right, c);
      case ">>>"        : return ev(left, c) >>>        ev(right, c);
      case "=="         : return ev(left, c) ==         ev(right, c);
      case "==="        : return ev(left, c) ===        ev(right, c);
      case "!="         : return ev(left, c) !=         ev(right, c);
      case "!=="        : return ev(left, c) !==        ev(right, c);
      case "<"          : return ev(left, c) <          ev(right, c);
      case "<="         : return ev(left, c) <=         ev(right, c);
      case ">"          : return ev(left, c) >          ev(right, c);
      case ">="         : return ev(left, c) >=         ev(right, c);
      case "in"         : return ev(left, c) in         ev(right, c);
      case "instanceof" : return ev(left, c) instanceof ev(right, c);
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Binary.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.left._walk(visitor);
        this.right._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.left.has_side_effects(compressor)
        || this.right.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Binary.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return member(this.operator, binary_bool) ||
        ( (this.operator == "&&" || this.operator == "||") &&
          this.left.is_boolean() && this.right.is_boolean() );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return this.operator == "+" &&
        (this.left.is_string(compressor) || this.right.is_string(compressor));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.lift_sequences"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.lift_sequences)
- description and source-code
```javascript
lift_sequences = function (compressor){
    if (compressor.option("sequences")) {
        if (this.left instanceof AST_Seq) {
            var seq = this.left;
            var x = seq.to_array();
            this.left = x.pop();
            x.push(this);
            seq = AST_Seq.from_array(x).transform(compressor);
            return seq;
        }
        if (this.right instanceof AST_Seq
            && this instanceof AST_Assign
            && !has_side_effects_or_prop_access(this.left, compressor)) {
            var seq = this.right;
            var x = seq.to_array();
            this.right = x.pop();
            x.push(this);
            seq = AST_Seq.from_array(x).transform(compressor);
            return seq;
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Binary.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    // (foo && bar)()
    if (p instanceof AST_Call && p.expression === this)
        return true;
    // typeof (foo && bar)
    if (p instanceof AST_Unary)
        return true;
    // (foo && bar)["prop"], (foo && bar).prop
    if (p instanceof AST_PropAccess && p.expression === this)
        return true;
    // this deals with precedence: 3 * (2 + 1)
    if (p instanceof AST_Binary) {
        var po = p.operator, pp = PRECEDENCE[po];
        var so = this.operator, sp = PRECEDENCE[so];
        if (pp > sp
            || (pp == sp
                && this === p.right)) {
            return true;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Binary.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Binary.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Binary.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Binary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Binary.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Block"></a>[module uglifyjs.AST_Block](#apidoc.module.uglifyjs.AST_Block)

#### <a name="apidoc.element.uglifyjs.AST_Block.AST_Block"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Block (props)](#apidoc.element.uglifyjs.AST_Block.AST_Block)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Block.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Block.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Block.SUBCLASSES"></a>[module uglifyjs.AST_Block.SUBCLASSES](#apidoc.module.uglifyjs.AST_Block.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.0)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.3)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.4)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.5)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.SUBCLASSES.6"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.SUBCLASSES.</span>6 (props)](#apidoc.element.uglifyjs.AST_Block.SUBCLASSES.6)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Block.prototype"></a>[module uglifyjs.AST_Block.prototype](#apidoc.module.uglifyjs.AST_Block.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Block.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Block.prototype.CTOR)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Block.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Block.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Block.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Block.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    for (var i = this.body.length; --i >= 0;) {
        if (this.body[i].has_side_effects(compressor))
            return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Block.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Block.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Block.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Block.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Block.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Block.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_BlockStatement"></a>[module uglifyjs.AST_BlockStatement](#apidoc.module.uglifyjs.AST_BlockStatement)

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.AST_BlockStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_BlockStatement (props)](#apidoc.element.uglifyjs.AST_BlockStatement.AST_BlockStatement)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_BlockStatement.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_BlockStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_BlockStatement.prototype"></a>[module uglifyjs.AST_BlockStatement.prototype](#apidoc.module.uglifyjs.AST_BlockStatement.prototype)

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_BlockStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.aborts)
- description and source-code
```javascript
function block_aborts(){
    var n = this.body.length;
    return n > 0 && aborts(this.body[n - 1]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_BlockStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_BlockStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_BlockStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Boolean"></a>[module uglifyjs.AST_Boolean](#apidoc.module.uglifyjs.AST_Boolean)

#### <a name="apidoc.element.uglifyjs.AST_Boolean.AST_Boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Boolean (props)](#apidoc.element.uglifyjs.AST_Boolean.AST_Boolean)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Boolean.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Boolean.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Boolean.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Boolean.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Boolean.SUBCLASSES"></a>[module uglifyjs.AST_Boolean.SUBCLASSES](#apidoc.module.uglifyjs.AST_Boolean.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Boolean.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Boolean.SUBCLASSES.0)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Boolean.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Boolean.SUBCLASSES.1)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Boolean.prototype"></a>[module uglifyjs.AST_Boolean.prototype](#apidoc.module.uglifyjs.AST_Boolean.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Boolean.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Boolean.prototype.CTOR)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Boolean.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Boolean.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Boolean.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Boolean.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Boolean.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Break"></a>[module uglifyjs.AST_Break](#apidoc.module.uglifyjs.AST_Break)

#### <a name="apidoc.element.uglifyjs.AST_Break.AST_Break"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Break (props)](#apidoc.element.uglifyjs.AST_Break.AST_Break)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Break.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Break.BASE)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Break.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Break.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Break.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Break.prototype"></a>[module uglifyjs.AST_Break.prototype](#apidoc.module.uglifyjs.AST_Break.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Break.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Break.prototype.CTOR)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Break.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Break.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "break");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Break.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Break.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Break.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Call"></a>[module uglifyjs.AST_Call](#apidoc.module.uglifyjs.AST_Call)

#### <a name="apidoc.element.uglifyjs.AST_Call.AST_Call"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Call (props)](#apidoc.element.uglifyjs.AST_Call.AST_Call)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Call.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Call.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Call.SUBCLASSES"></a>[module uglifyjs.AST_Call.SUBCLASSES](#apidoc.module.uglifyjs.AST_Call.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Call.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Call.SUBCLASSES.0)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Call.prototype"></a>[module uglifyjs.AST_Call.prototype](#apidoc.module.uglifyjs.AST_Call.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Call.prototype.CTOR)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Call.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.expression.print(output);
    if (self instanceof AST_New && no_constructor_parens(self, output))
        return;
    output.with_parens(function(){
        self.args.forEach(function(expr, i){
            if (i) output.comma();
            expr.print(output);
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Call.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        this.args.forEach(function(arg){
            arg._walk(visitor);
        });
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Call.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    var pure = compressor.option("pure_funcs");
    if (!pure) return true;
    return pure.indexOf(this.expression.print_to_string()) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Call.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return compressor.option("unsafe")
        && this.expression instanceof AST_SymbolRef
        && this.expression.name == "String"
        && this.expression.undeclared();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Call.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent(), p1;
    if (p instanceof AST_New && p.expression === this)
        return true;

    // workaround for Safari bug.
    // https://bugs.webkit.org/show_bug.cgi?id=123506
    return this.expression instanceof AST_Function
        && p instanceof AST_PropAccess
        && p.expression === this
        && (p1 = output.parent(1)) instanceof AST_Assign
        && p1.left === p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Call.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Call.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Call.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Call.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Call.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Case"></a>[module uglifyjs.AST_Case](#apidoc.module.uglifyjs.AST_Case)

#### <a name="apidoc.element.uglifyjs.AST_Case.AST_Case"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Case (props)](#apidoc.element.uglifyjs.AST_Case.AST_Case)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Case.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Case.BASE)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Case.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Case.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Case.prototype"></a>[module uglifyjs.AST_Case.prototype](#apidoc.module.uglifyjs.AST_Case.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Case.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Case.prototype.CTOR)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Case.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Case.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("case");
    output.space();
    self.expression.print(output);
    output.print(":");
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Case.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Case.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Case.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Case.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Case.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Case.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Case.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Catch"></a>[module uglifyjs.AST_Catch](#apidoc.module.uglifyjs.AST_Catch)

#### <a name="apidoc.element.uglifyjs.AST_Catch.AST_Catch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Catch (props)](#apidoc.element.uglifyjs.AST_Catch.AST_Catch)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Catch.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Catch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Catch.prototype"></a>[module uglifyjs.AST_Catch.prototype](#apidoc.module.uglifyjs.AST_Catch.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Catch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Catch.prototype.CTOR)
- description and source-code
```javascript
function AST_Catch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.argname = props
.argname;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Catch.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("catch");
    output.space();
    output.with_parens(function(){
        self.argname.print(output);
    });
    output.space();
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Catch.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.argname._walk(visitor);
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Catch.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Catch.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Catch.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Catch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Catch.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Conditional"></a>[module uglifyjs.AST_Conditional](#apidoc.module.uglifyjs.AST_Conditional)

#### <a name="apidoc.element.uglifyjs.AST_Conditional.AST_Conditional"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Conditional (props)](#apidoc.element.uglifyjs.AST_Conditional.AST_Conditional)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Conditional.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Conditional.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Conditional.prototype"></a>[module uglifyjs.AST_Conditional.prototype](#apidoc.module.uglifyjs.AST_Conditional.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Conditional.prototype.CTOR)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Conditional.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.condition.print(output);
    output.space();
    output.print("?");
    output.space();
    self.consequent.print(output);
    output.space();
    output.colon();
    self.alternative.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    return ev(this.condition, compressor)
        ? ev(this.consequent, compressor)
        : ev(this.alternative, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Conditional.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.condition._walk(visitor);
        this.consequent._walk(visitor);
        this.alternative._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.condition.has_side_effects(compressor)
        || this.consequent.has_side_effects(compressor)
        || this.alternative.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Conditional.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return this.consequent.is_boolean() && this.alternative.is_boolean();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return this.consequent.is_string(compressor) && this.alternative.is_string(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Conditional.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    // !(a = false) → true
    if (p instanceof AST_Unary)
        return true;
    // 1 + (a = 2) + 3 → 6, side effect setting a = 2
    if (p instanceof AST_Binary && !(p instanceof AST_Assign))
        return true;
    // (a = func)() —or— new (a = Object)()
    if (p instanceof AST_Call && p.expression === this)
        return true;
    // (a = foo) ? bar : baz
    if (p instanceof AST_Conditional && p.condition === this)
        return true;
    // (a = foo)["prop"] —or— (a = foo).prop
    if (p instanceof AST_PropAccess && p.expression === this)
        return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Conditional.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Conditional.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Conditional.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Conditional.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Conditional.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Const"></a>[module uglifyjs.AST_Const](#apidoc.module.uglifyjs.AST_Const)

#### <a name="apidoc.element.uglifyjs.AST_Const.AST_Const"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Const (props)](#apidoc.element.uglifyjs.AST_Const.AST_Const)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Const.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Const.BASE)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Const.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Const.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Const.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Const.prototype"></a>[module uglifyjs.AST_Const.prototype](#apidoc.module.uglifyjs.AST_Const.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Const.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Const.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Const.prototype.CTOR)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Const.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Const.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Const.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "const");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Constant"></a>[module uglifyjs.AST_Constant](#apidoc.module.uglifyjs.AST_Constant)

#### <a name="apidoc.element.uglifyjs.AST_Constant.AST_Constant"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Constant (props)](#apidoc.element.uglifyjs.AST_Constant.AST_Constant)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Constant.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Constant.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Constant.SUBCLASSES"></a>[module uglifyjs.AST_Constant.SUBCLASSES](#apidoc.module.uglifyjs.AST_Constant.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.0)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.2)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Constant.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Constant.prototype"></a>[module uglifyjs.AST_Constant.prototype](#apidoc.module.uglifyjs.AST_Constant.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Constant.prototype.CTOR)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Constant.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print(self.getValue());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Constant.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    return this.getValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Constant.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype.getValue"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>getValue ()](#apidoc.element.uglifyjs.AST_Constant.prototype.getValue)
- description and source-code
```javascript
getValue = function () {
    return this.value;
}
```
- example usage
```shell
...
    }));
}
var wrapped_tl = "(function(exports, global){ global['" + name + "'] = exports; '$ORIG'; '$EXPORTS'; }({}, (function(){return this
}())))";
wrapped_tl = parse(wrapped_tl);
wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
    if (node instanceof AST_SimpleStatement) {
        node = node.body;
        if (node instanceof AST_String) switch (node.getValue()) {
          case "$ORIG":
            return MAP.splice(self.body);
          case "$EXPORTS":
            var body = [];
            to_export.forEach(function(sym){
                body.push(new AST_SimpleStatement({
                    body: new AST_Assign({
...
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Constant.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return false }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Constant.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Constant.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Constant.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Continue"></a>[module uglifyjs.AST_Continue](#apidoc.module.uglifyjs.AST_Continue)

#### <a name="apidoc.element.uglifyjs.AST_Continue.AST_Continue"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Continue (props)](#apidoc.element.uglifyjs.AST_Continue.AST_Continue)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Continue.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Continue.BASE)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Continue.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Continue.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Continue.prototype"></a>[module uglifyjs.AST_Continue.prototype](#apidoc.module.uglifyjs.AST_Continue.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Continue.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Continue.prototype.CTOR)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Continue.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Continue.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "continue");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Continue.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Continue.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Continue.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_DWLoop"></a>[module uglifyjs.AST_DWLoop](#apidoc.module.uglifyjs.AST_DWLoop)

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.AST_DWLoop"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_DWLoop (props)](#apidoc.element.uglifyjs.AST_DWLoop.AST_DWLoop)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>BASE (props)](#apidoc.element.uglifyjs.AST_DWLoop.BASE)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_DWLoop.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_DWLoop.SUBCLASSES"></a>[module uglifyjs.AST_DWLoop.SUBCLASSES](#apidoc.module.uglifyjs.AST_DWLoop.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_DWLoop.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_DWLoop.SUBCLASSES.1)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_DWLoop.prototype"></a>[module uglifyjs.AST_DWLoop.prototype](#apidoc.module.uglifyjs.AST_DWLoop.prototype)

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_DWLoop.prototype.CTOR)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_DWLoop.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_DWLoop.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_DWLoop.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_DWLoop.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Debugger"></a>[module uglifyjs.AST_Debugger](#apidoc.module.uglifyjs.AST_Debugger)

#### <a name="apidoc.element.uglifyjs.AST_Debugger.AST_Debugger"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Debugger (props)](#apidoc.element.uglifyjs.AST_Debugger.AST_Debugger)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Debugger.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Debugger.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Debugger.prototype"></a>[module uglifyjs.AST_Debugger.prototype](#apidoc.module.uglifyjs.AST_Debugger.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Debugger.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Debugger.prototype.CTOR)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Debugger.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("debugger");
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Debugger.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Debugger.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Debugger.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Debugger.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Debugger.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Default"></a>[module uglifyjs.AST_Default](#apidoc.module.uglifyjs.AST_Default)

#### <a name="apidoc.element.uglifyjs.AST_Default.AST_Default"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Default (props)](#apidoc.element.uglifyjs.AST_Default.AST_Default)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Default.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Default.BASE)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Default.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Default.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Default.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Default.prototype"></a>[module uglifyjs.AST_Default.prototype](#apidoc.module.uglifyjs.AST_Default.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Default.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Default.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Default.prototype.CTOR)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Default.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Default.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Default.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("default:");
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Definitions"></a>[module uglifyjs.AST_Definitions](#apidoc.module.uglifyjs.AST_Definitions)

#### <a name="apidoc.element.uglifyjs.AST_Definitions.AST_Definitions"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Definitions (props)](#apidoc.element.uglifyjs.AST_Definitions.AST_Definitions)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Definitions.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Definitions.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Definitions.SUBCLASSES"></a>[module uglifyjs.AST_Definitions.SUBCLASSES](#apidoc.module.uglifyjs.AST_Definitions.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Definitions.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Definitions.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Definitions.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Const(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Definitions.prototype"></a>[module uglifyjs.AST_Definitions.prototype](#apidoc.module.uglifyjs.AST_Definitions.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Definitions.prototype.CTOR)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>_do_print (output, kind)](#apidoc.element.uglifyjs.AST_Definitions.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, kind){
    output.print(kind);
    output.space();
    this.definitions.forEach(function(def, i){
        if (i) output.comma();
        def.print(output);
    });
    var p = output.parent();
    var in_for = p instanceof AST_For || p instanceof AST_ForIn;
    var avoid_semicolon = in_for && p.init === this;
    if (!avoid_semicolon)
        output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Definitions.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.definitions.forEach(function(def){
            def._walk(visitor);
        });
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Definitions.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Definitions.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.remove_initializers"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>remove_initializers ()](#apidoc.element.uglifyjs.AST_Definitions.prototype.remove_initializers)
- description and source-code
```javascript
remove_initializers = function (){
    this.definitions.forEach(function(def){ def.value = null });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.to_assignments"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>to_assignments ()](#apidoc.element.uglifyjs.AST_Definitions.prototype.to_assignments)
- description and source-code
```javascript
to_assignments = function (){
    var assignments = this.definitions.reduce(function(a, def){
        if (def.value) {
            var name = make_node(AST_SymbolRef, def.name, def.name);
            a.push(make_node(AST_Assign, def, {
                operator : "=",
                left     : name,
                right    : def.value
            }));
        }
        return a;
    }, []);
    if (assignments.length == 0) return null;
    return AST_Seq.from_array(assignments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Definitions.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Definitions.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Definitions.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Definitions.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Defun"></a>[module uglifyjs.AST_Defun](#apidoc.module.uglifyjs.AST_Defun)

#### <a name="apidoc.element.uglifyjs.AST_Defun.AST_Defun"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Defun (props)](#apidoc.element.uglifyjs.AST_Defun.AST_Defun)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Defun.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Defun.BASE)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Defun.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Defun.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Defun.prototype"></a>[module uglifyjs.AST_Defun.prototype](#apidoc.module.uglifyjs.AST_Defun.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Defun.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Defun.prototype.CTOR)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Defun.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Defun.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return true }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Defun.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Defun.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Defun.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Directive"></a>[module uglifyjs.AST_Directive](#apidoc.module.uglifyjs.AST_Directive)

#### <a name="apidoc.element.uglifyjs.AST_Directive.AST_Directive"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Directive (props)](#apidoc.element.uglifyjs.AST_Directive.AST_Directive)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Directive.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Directive.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Directive.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Directive.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Directive.prototype"></a>[module uglifyjs.AST_Directive.prototype](#apidoc.module.uglifyjs.AST_Directive.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Directive.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Directive.prototype.CTOR)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Directive.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Directive.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print_string(self.value, self.quote);
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Directive.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Directive.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Directive.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Directive.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Directive.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Directive.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Directive.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Do"></a>[module uglifyjs.AST_Do](#apidoc.module.uglifyjs.AST_Do)

#### <a name="apidoc.element.uglifyjs.AST_Do.AST_Do"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Do (props)](#apidoc.element.uglifyjs.AST_Do.AST_Do)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Do.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Do.BASE)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Do.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Do.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Do.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Do.prototype"></a>[module uglifyjs.AST_Do.prototype](#apidoc.module.uglifyjs.AST_Do.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Do.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Do.prototype.CTOR)
- description and source-code
```javascript
function AST_Do(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Do.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Do.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("do");
    output.space();
    self._do_print_body(output);
    output.space();
    output.print("while");
    output.space();
    output.with_parens(function(){
        self.condition.print(output);
    });
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Do.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Do.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.body._walk(visitor);
        this.condition._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Do.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Do.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Do.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Dot"></a>[module uglifyjs.AST_Dot](#apidoc.module.uglifyjs.AST_Dot)

#### <a name="apidoc.element.uglifyjs.AST_Dot.AST_Dot"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Dot (props)](#apidoc.element.uglifyjs.AST_Dot.AST_Dot)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Dot.BASE)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Dot.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Dot.prototype"></a>[module uglifyjs.AST_Dot.prototype](#apidoc.module.uglifyjs.AST_Dot.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Dot.prototype.CTOR)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Dot.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var expr = self.expression;
    expr.print(output);
    if (expr instanceof AST_Number && expr.getValue() >= 0) {
        if (!/[xa-f.]/i.test(output.last())) {
            output.print(".");
        }
    }
    output.print(".");
    // the name after dot would be mapped about here.
    output.add_mapping(self.end);
    output.print_name(self.property);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_Dot.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    if (compressor.option("unsafe") && this.property == "length") {
        var str = ev(this.expression, compressor);
        if (typeof str == "string")
            return str.length;
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Dot.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Dot.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    if (!compressor.option("pure_getters")) return true;
    return this.expression.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Dot.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Dot.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Dot.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Dot.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_EmptyStatement"></a>[module uglifyjs.AST_EmptyStatement](#apidoc.module.uglifyjs.AST_EmptyStatement)

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.AST_EmptyStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_EmptyStatement (props)](#apidoc.element.uglifyjs.AST_EmptyStatement.AST_EmptyStatement)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_EmptyStatement.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_EmptyStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_EmptyStatement.prototype"></a>[module uglifyjs.AST_EmptyStatement.prototype](#apidoc.module.uglifyjs.AST_EmptyStatement.prototype)

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this);
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return false }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_EmptyStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_EmptyStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_EmptyStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Exit"></a>[module uglifyjs.AST_Exit](#apidoc.module.uglifyjs.AST_Exit)

#### <a name="apidoc.element.uglifyjs.AST_Exit.AST_Exit"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Exit (props)](#apidoc.element.uglifyjs.AST_Exit.AST_Exit)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Exit.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Exit.BASE)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Exit.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Exit.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Exit.SUBCLASSES"></a>[module uglifyjs.AST_Exit.SUBCLASSES](#apidoc.module.uglifyjs.AST_Exit.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Exit.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Exit.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Exit.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Exit.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Exit.prototype"></a>[module uglifyjs.AST_Exit.prototype](#apidoc.module.uglifyjs.AST_Exit.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Exit.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Exit.prototype.CTOR)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Exit.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>_do_print (output, kind)](#apidoc.element.uglifyjs.AST_Exit.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, kind){
    output.print(kind);
    if (this.value) {
        output.space();
        this.value.print(output);
    }
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Exit.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Exit.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, this.value && function(){
        this.value._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Exit.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Exit.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Exit.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_False"></a>[module uglifyjs.AST_False](#apidoc.module.uglifyjs.AST_False)

#### <a name="apidoc.element.uglifyjs.AST_False.AST_False"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_False (props)](#apidoc.element.uglifyjs.AST_False.AST_False)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_False.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>BASE (props)](#apidoc.element.uglifyjs.AST_False.BASE)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_False.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_False.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_False.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_False.prototype"></a>[module uglifyjs.AST_False.prototype](#apidoc.module.uglifyjs.AST_False.prototype)

#### <a name="apidoc.element.uglifyjs.AST_False.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_False.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_False.prototype.CTOR)
- description and source-code
```javascript
function AST_False(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_False.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_False.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_False.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){ return true }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Finally"></a>[module uglifyjs.AST_Finally](#apidoc.module.uglifyjs.AST_Finally)

#### <a name="apidoc.element.uglifyjs.AST_Finally.AST_Finally"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Finally (props)](#apidoc.element.uglifyjs.AST_Finally.AST_Finally)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Finally.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Finally.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Finally.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Finally.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Finally.prototype"></a>[module uglifyjs.AST_Finally.prototype](#apidoc.module.uglifyjs.AST_Finally.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Finally.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Finally.prototype.CTOR)
- description and source-code
```javascript
function AST_Finally(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Finally.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Finally.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("finally");
    output.space();
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Finally.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Finally.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Finally.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_For"></a>[module uglifyjs.AST_For](#apidoc.module.uglifyjs.AST_For)

#### <a name="apidoc.element.uglifyjs.AST_For.AST_For"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_For (props)](#apidoc.element.uglifyjs.AST_For.AST_For)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_For.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>BASE (props)](#apidoc.element.uglifyjs.AST_For.BASE)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_For.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_For.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_For.prototype"></a>[module uglifyjs.AST_For.prototype](#apidoc.module.uglifyjs.AST_For.prototype)

#### <a name="apidoc.element.uglifyjs.AST_For.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_For.prototype.CTOR)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_For.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_For.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("for");
    output.space();
    output.with_parens(function(){
        if (self.init && !(self.init instanceof AST_EmptyStatement)) {
            if (self.init instanceof AST_Definitions) {
                self.init.print(output);
            } else {
                parenthesize_for_noin(self.init, output, true);
            }
            output.print(";");
            output.space();
        } else {
            output.print(";");
        }
        if (self.condition) {
            self.condition.print(output);
            output.print(";");
            output.space();
        } else {
            output.print(";");
        }
        if (self.step) {
            self.step.print(output);
        }
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_For.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_For.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        if (this.init) this.init._walk(visitor);
        if (this.condition) this.condition._walk(visitor);
        if (this.step) this.step._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_For.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_For.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_For.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_For.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_For.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_For.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_For.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_ForIn"></a>[module uglifyjs.AST_ForIn](#apidoc.module.uglifyjs.AST_ForIn)

#### <a name="apidoc.element.uglifyjs.AST_ForIn.AST_ForIn"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ForIn (props)](#apidoc.element.uglifyjs.AST_ForIn.AST_ForIn)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ForIn.BASE)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ForIn.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ForIn.prototype"></a>[module uglifyjs.AST_ForIn.prototype](#apidoc.module.uglifyjs.AST_ForIn.prototype)

#### <a name="apidoc.element.uglifyjs.AST_ForIn.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ForIn.prototype.CTOR)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ForIn.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("for");
    output.space();
    output.with_parens(function(){
        self.init.print(output);
        output.space();
        output.print("in");
        output.space();
        self.object.print(output);
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_ForIn.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.init._walk(visitor);
        this.object._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_ForIn.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_ForIn.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ForIn.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_ForIn.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Function"></a>[module uglifyjs.AST_Function](#apidoc.module.uglifyjs.AST_Function)

#### <a name="apidoc.element.uglifyjs.AST_Function.AST_Function"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Function (props)](#apidoc.element.uglifyjs.AST_Function.AST_Function)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Function.BASE)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Function.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Function.prototype"></a>[module uglifyjs.AST_Function.prototype](#apidoc.module.uglifyjs.AST_Function.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Function.prototype.CTOR)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Function.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    // XXX: AST_Function inherits from AST_Scope, which itself
    // inherits from AST_Statement; however, an AST_Function
    // isn't really a statement.  This could byte in other
    // places too. :-( Wish JS had multiple inheritance.
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Function.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return false }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Function.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    return first_in_statement(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Function.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.next_mangled"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>next_mangled (options, def)](#apidoc.element.uglifyjs.AST_Function.prototype.next_mangled)
- description and source-code
```javascript
next_mangled = function (options, def){
    // #179, #326
    // in Safari strict mode, something like (function x(x){...}) is a syntax error;
    // a function expression's argument cannot shadow the function expression's name

    var tricky_def = def.orig[0] instanceof AST_SymbolFunarg && this.name && this.name.definition();
    while (true) {
        var name = AST_Lambda.prototype.next_mangled.call(this, options, def);
        if (!(tricky_def && tricky_def.mangled_name == name))
            return name;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Function.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Function.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Function.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Function.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Hole"></a>[module uglifyjs.AST_Hole](#apidoc.module.uglifyjs.AST_Hole)

#### <a name="apidoc.element.uglifyjs.AST_Hole.AST_Hole"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Hole (props)](#apidoc.element.uglifyjs.AST_Hole.AST_Hole)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Hole.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Hole.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Hole.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Hole.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Hole.prototype"></a>[module uglifyjs.AST_Hole.prototype](#apidoc.module.uglifyjs.AST_Hole.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Hole.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Hole.prototype.CTOR)
- description and source-code
```javascript
function AST_Hole(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Hole.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>_codegen ()](#apidoc.element.uglifyjs.AST_Hole.prototype._codegen)
- description and source-code
```javascript
function noop() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Hole.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Hole.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Hole.prototype.to_mozilla_ast)
- description and source-code
```javascript
function To_Moz_ArrayHole() { return null }
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_If"></a>[module uglifyjs.AST_If](#apidoc.module.uglifyjs.AST_If)

#### <a name="apidoc.element.uglifyjs.AST_If.AST_If"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_If (props)](#apidoc.element.uglifyjs.AST_If.AST_If)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_If.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>BASE (props)](#apidoc.element.uglifyjs.AST_If.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_If.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_If.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_If.prototype"></a>[module uglifyjs.AST_If.prototype](#apidoc.module.uglifyjs.AST_If.prototype)

#### <a name="apidoc.element.uglifyjs.AST_If.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_If.prototype.CTOR)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_If.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_If.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("if");
    output.space();
    output.with_parens(function(){
        self.condition.print(output);
    });
    output.space();
    if (self.alternative) {
        make_then(self, output);
        output.space();
        output.print("else");
        output.space();
        force_statement(self.alternative, output);
    } else {
        self._do_print_body(output);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_If.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_If.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.condition._walk(visitor);
        this.body._walk(visitor);
        if (this.alternative) this.alternative._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_If.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_If.prototype.aborts)
- description and source-code
```javascript
aborts = function (){
    return this.alternative && aborts(this.body) && aborts(this.alternative) && this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_If.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_If.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_If.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_If.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_If.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_If.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_If.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Infinity"></a>[module uglifyjs.AST_Infinity](#apidoc.module.uglifyjs.AST_Infinity)

#### <a name="apidoc.element.uglifyjs.AST_Infinity.AST_Infinity"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Infinity (props)](#apidoc.element.uglifyjs.AST_Infinity.AST_Infinity)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Infinity.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Infinity.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Infinity.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Infinity.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Infinity.prototype"></a>[module uglifyjs.AST_Infinity.prototype](#apidoc.module.uglifyjs.AST_Infinity.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Infinity.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Infinity.prototype.CTOR)
- description and source-code
```javascript
function AST_Infinity(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Infinity.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Infinity.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("Infinity");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Infinity.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Infinity.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Infinity.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_IterationStatement"></a>[module uglifyjs.AST_IterationStatement](#apidoc.module.uglifyjs.AST_IterationStatement)

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.AST_IterationStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_IterationStatement (props)](#apidoc.element.uglifyjs.AST_IterationStatement.AST_IterationStatement)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_IterationStatement.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_IterationStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_IterationStatement.SUBCLASSES"></a>[module uglifyjs.AST_IterationStatement.SUBCLASSES](#apidoc.module.uglifyjs.AST_IterationStatement.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.0)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.1)
- description and source-code
```javascript
function AST_For(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.step = props.step
;this.condition = props.condition;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_IterationStatement.SUBCLASSES.2)
- description and source-code
```javascript
function AST_ForIn(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.object = props
.object;this.name = props.name;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_IterationStatement.prototype"></a>[module uglifyjs.AST_IterationStatement.prototype](#apidoc.module.uglifyjs.AST_IterationStatement.prototype)

#### <a name="apidoc.element.uglifyjs.AST_IterationStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_IterationStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_IterationStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_Jump"></a>[module uglifyjs.AST_Jump](#apidoc.module.uglifyjs.AST_Jump)

#### <a name="apidoc.element.uglifyjs.AST_Jump.AST_Jump"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Jump (props)](#apidoc.element.uglifyjs.AST_Jump.AST_Jump)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Jump.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Jump.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Jump.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Jump.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Jump.SUBCLASSES"></a>[module uglifyjs.AST_Jump.SUBCLASSES](#apidoc.module.uglifyjs.AST_Jump.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Jump.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Jump.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Jump.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Jump.SUBCLASSES.1)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Jump.prototype"></a>[module uglifyjs.AST_Jump.prototype](#apidoc.module.uglifyjs.AST_Jump.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Jump.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Jump.prototype.CTOR)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Jump.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_Jump.prototype.aborts)
- description and source-code
```javascript
aborts = function (){ return this }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Jump.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Jump.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Jump.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Label"></a>[module uglifyjs.AST_Label](#apidoc.module.uglifyjs.AST_Label)

#### <a name="apidoc.element.uglifyjs.AST_Label.AST_Label"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Label (props)](#apidoc.element.uglifyjs.AST_Label.AST_Label)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Label.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Label.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Label.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Label.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Label.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Label.prototype"></a>[module uglifyjs.AST_Label.prototype](#apidoc.module.uglifyjs.AST_Label.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Label.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Label.prototype.CTOR)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Label.prototype.initialize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>initialize ()](#apidoc.element.uglifyjs.AST_Label.prototype.initialize)
- description and source-code
```javascript
initialize = function () {
    this.references = [];
    this.thedef = this;
}
```
- example usage
```shell
...
    props = props.concat(base.PROPS);
var code = "return function AST_" + type + "(props){ if (props) { ";
for (var i = props.length; --i >= 0;) {
    code += "this." + props[i] + " = props." + props[i] + ";";
}
var proto = base && new base;
if (proto && proto.initialize || (methods && methods.initialize))
    code += "this.initialize();";
code += "}}";
var ctor = new Function(code)();
if (proto) {
    ctor.prototype = proto;
    ctor.BASE = base;
}
if (base) base.SUBCLASSES.push(ctor);
...
```

#### <a name="apidoc.element.uglifyjs.AST_Label.prototype.undeclared"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>undeclared ()](#apidoc.element.uglifyjs.AST_Label.prototype.undeclared)
- description and source-code
```javascript
undeclared = function (){
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Label.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Label.prototype.</span>unmangleable ()](#apidoc.element.uglifyjs.AST_Label.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (){
    return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_LabelRef"></a>[module uglifyjs.AST_LabelRef](#apidoc.module.uglifyjs.AST_LabelRef)

#### <a name="apidoc.element.uglifyjs.AST_LabelRef.AST_LabelRef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabelRef (props)](#apidoc.element.uglifyjs.AST_LabelRef.AST_LabelRef)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabelRef.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>BASE (props)](#apidoc.element.uglifyjs.AST_LabelRef.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabelRef.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_LabelRef.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_LabelRef.prototype"></a>[module uglifyjs.AST_LabelRef.prototype](#apidoc.module.uglifyjs.AST_LabelRef.prototype)

#### <a name="apidoc.element.uglifyjs.AST_LabelRef.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_LabelRef.prototype.CTOR)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_LabelRef.prototype.undeclared"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabelRef.prototype.</span>undeclared ()](#apidoc.element.uglifyjs.AST_LabelRef.prototype.undeclared)
- description and source-code
```javascript
undeclared = function (){
    return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_LabeledStatement"></a>[module uglifyjs.AST_LabeledStatement](#apidoc.module.uglifyjs.AST_LabeledStatement)

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.AST_LabeledStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LabeledStatement (props)](#apidoc.element.uglifyjs.AST_LabeledStatement.AST_LabeledStatement)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_LabeledStatement.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_LabeledStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_LabeledStatement.prototype"></a>[module uglifyjs.AST_LabeledStatement.prototype](#apidoc.module.uglifyjs.AST_LabeledStatement.prototype)

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.label.print(output);
    output.colon();
    self.body.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.label._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_LabeledStatement.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LabeledStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_LabeledStatement.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Lambda"></a>[module uglifyjs.AST_Lambda](#apidoc.module.uglifyjs.AST_Lambda)

#### <a name="apidoc.element.uglifyjs.AST_Lambda.AST_Lambda"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Lambda (props)](#apidoc.element.uglifyjs.AST_Lambda.AST_Lambda)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Lambda.BASE)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Lambda.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Lambda.SUBCLASSES"></a>[module uglifyjs.AST_Lambda.SUBCLASSES](#apidoc.module.uglifyjs.AST_Lambda.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Accessor(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Function(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Lambda.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Defun(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Lambda.prototype"></a>[module uglifyjs.AST_Lambda.prototype](#apidoc.module.uglifyjs.AST_Lambda.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Lambda.prototype.CTOR)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Lambda.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>_do_print (output, nokeyword)](#apidoc.element.uglifyjs.AST_Lambda.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, nokeyword){
    var self = this;
    if (!nokeyword) {
        output.print("function");
    }
    if (self.name) {
        output.space();
        self.name.print(output);
    }
    output.with_parens(function(){
        self.argnames.forEach(function(arg, i){
            if (i) output.comma();
            arg.print(output);
        });
    });
    output.space();
    print_bracketed(self.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Lambda.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        if (this.name) this.name._walk(visitor);
        this.argnames.forEach(function(arg){
            arg._walk(visitor);
        });
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Lambda.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype.init_scope_vars"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>init_scope_vars ()](#apidoc.element.uglifyjs.AST_Lambda.prototype.init_scope_vars)
- description and source-code
```javascript
init_scope_vars = function (){
    AST_Scope.prototype.init_scope_vars.apply(this, arguments);
    this.uses_arguments = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Lambda.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Lambda.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Lambda.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Lambda.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_LoopControl"></a>[module uglifyjs.AST_LoopControl](#apidoc.module.uglifyjs.AST_LoopControl)

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.AST_LoopControl"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_LoopControl (props)](#apidoc.element.uglifyjs.AST_LoopControl.AST_LoopControl)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>BASE (props)](#apidoc.element.uglifyjs.AST_LoopControl.BASE)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_LoopControl.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_LoopControl.SUBCLASSES"></a>[module uglifyjs.AST_LoopControl.SUBCLASSES](#apidoc.module.uglifyjs.AST_LoopControl.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_LoopControl.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Break(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_LoopControl.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Continue(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_LoopControl.prototype"></a>[module uglifyjs.AST_LoopControl.prototype](#apidoc.module.uglifyjs.AST_LoopControl.prototype)

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_LoopControl.prototype.CTOR)
- description and source-code
```javascript
function AST_LoopControl(props){ if (props) { this.end = props.end;this.start = props.start;this.label = props.label;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>_do_print (output, kind)](#apidoc.element.uglifyjs.AST_LoopControl.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output, kind){
    output.print(kind);
    if (this.label) {
        output.space();
        this.label.print(output);
    }
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_LoopControl.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, this.label && function(){
        this.label._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_LoopControl.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_LoopControl.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_LoopControl.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_NaN"></a>[module uglifyjs.AST_NaN](#apidoc.module.uglifyjs.AST_NaN)

#### <a name="apidoc.element.uglifyjs.AST_NaN.AST_NaN"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_NaN (props)](#apidoc.element.uglifyjs.AST_NaN.AST_NaN)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_NaN.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>BASE (props)](#apidoc.element.uglifyjs.AST_NaN.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_NaN.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_NaN.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_NaN.prototype"></a>[module uglifyjs.AST_NaN.prototype](#apidoc.module.uglifyjs.AST_NaN.prototype)

#### <a name="apidoc.element.uglifyjs.AST_NaN.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_NaN.prototype.CTOR)
- description and source-code
```javascript
function AST_NaN(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_NaN.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_NaN.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("NaN");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_NaN.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_NaN.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_NaN.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_New"></a>[module uglifyjs.AST_New](#apidoc.module.uglifyjs.AST_New)

#### <a name="apidoc.element.uglifyjs.AST_New.AST_New"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_New (props)](#apidoc.element.uglifyjs.AST_New.AST_New)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>BASE (props)](#apidoc.element.uglifyjs.AST_New.BASE)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_New.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_New.prototype"></a>[module uglifyjs.AST_New.prototype](#apidoc.module.uglifyjs.AST_New.prototype)

#### <a name="apidoc.element.uglifyjs.AST_New.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_New.prototype.CTOR)
- description and source-code
```javascript
function AST_New(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_New.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_New.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("new");
    output.space();
    AST_Call.prototype._codegen(self, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_New.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_New.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    if (no_constructor_parens(this, output)
        && (p instanceof AST_PropAccess // (new Date).getTime(), (new Date)["getTime"]()
            || p instanceof AST_Call && p.expression === this)) // (new foo)(bar)
        return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_New.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_New.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_New.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_New.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Node"></a>[module uglifyjs.AST_Node](#apidoc.module.uglifyjs.AST_Node)

#### <a name="apidoc.element.uglifyjs.AST_Node.AST_Node"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Node (props)](#apidoc.element.uglifyjs.AST_Node.AST_Node)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Node.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.from_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>from_mozilla_ast (node)](#apidoc.element.uglifyjs.AST_Node.from_mozilla_ast)
- description and source-code
```javascript
from_mozilla_ast = function (node){
    var save_stack = FROM_MOZ_STACK;
    FROM_MOZ_STACK = [];
    var ast = from_moz(node);
    FROM_MOZ_STACK = save_stack;
    return ast;
}
```
- example usage
```shell
...
JavaScript ASTs in SpiderMonkey format.

Example:

'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.warn"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>warn (txt, props)](#apidoc.element.uglifyjs.AST_Node.warn)
- description and source-code
```javascript
warn = function (txt, props) {
    if (AST_Node.warn_function)
        AST_Node.warn_function(string_template(txt, props));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.warn_function"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.</span>warn_function (txt)](#apidoc.element.uglifyjs.AST_Node.warn_function)
- description and source-code
```javascript
warn_function = function (txt) {
    sys.error("WARN: " + txt);
}
```
- example usage
```shell
...
        return this._walk(visitor); // not sure the indirection will be any help
    }
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
    if (AST_Node.warn_function)
        AST_Node.warn_function(string_template(txt, props));
};

/* -----[ statements ]----- */

var AST_Statement = DEFNODE("Statement", null, {
    $documentation: "Base class of all statements",
});
...
```



# <a name="apidoc.module.uglifyjs.AST_Node.SUBCLASSES"></a>[module uglifyjs.AST_Node.SUBCLASSES](#apidoc.module.uglifyjs.AST_Node.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.1)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.10"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>10 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.10)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.11"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>11 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.11)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.12"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>12 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.12)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Call(props){ if (props) { this.end = props.end;this.start = props.start;this.args = props.args;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.4)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.5)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.6"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>6 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.6)
- description and source-code
```javascript
function AST_Binary(props){ if (props) { this.end = props.end;this.start = props.start;this.right = props.right;this.operator =
props.operator;this.left = props.left;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.7"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>7 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.7)
- description and source-code
```javascript
function AST_Conditional(props){ if (props) { this.end = props.end;this.start = props.start;this.alternative = props.alternative
;this.consequent = props.consequent;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.8"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>8 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.8)
- description and source-code
```javascript
function AST_Array(props){ if (props) { this.end = props.end;this.start = props.start;this.elements = props.elements;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.SUBCLASSES.9"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.SUBCLASSES.</span>9 (props)](#apidoc.element.uglifyjs.AST_Node.SUBCLASSES.9)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Node.prototype"></a>[module uglifyjs.AST_Node.prototype](#apidoc.module.uglifyjs.AST_Node.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Node.prototype.CTOR)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Node.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    throw def;          // not constant
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Node.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this);
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.add_comments"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>add_comments (output)](#apidoc.element.uglifyjs.AST_Node.prototype.add_comments)
- description and source-code
```javascript
add_comments = function (output){
    var c = output.option("comments"), self = this;
    if (c) {
        var start = self.start;
        if (start && !start._comments_dumped) {
            start._comments_dumped = true;
            var comments = start.comments_before || [];

            // XXX: ugly fix for https://github.com/mishoo/UglifyJS2/issues/112
            //               and https://github.com/mishoo/UglifyJS2/issues/372
            if (self instanceof AST_Exit && self.value) {
                self.value.walk(new TreeWalker(function(node){
                    if (node.start && node.start.comments_before) {
                        comments = comments.concat(node.start.comments_before);
                        node.start.comments_before = [];
                    }
                    if (node instanceof AST_Function ||
                        node instanceof AST_Array ||
                        node instanceof AST_Object)
                    {
                        return true; // don't go inside.
                    }
                }));
            }

            if (c.test) {
                comments = comments.filter(function(comment){
                    return c.test(comment.value);
                });
            } else if (typeof c == "function") {
                comments = comments.filter(function(comment){
                    return c(self, comment);
                });
            }

            // Keep single line comments after nlb, after nlb
            if (!output.option("beautify") && comments.length > 0 &&
                /comment[134]/.test(comments[0].type) &&
                output.col() !== 0 && comments[0].nlb)
            {
                output.print("\n");
            }

            comments.forEach(function(c){
                if (/comment[134]/.test(c.type)) {
                    output.print("//" + c.value + "\n");
                    output.indent();
                }
                else if (c.type == "comment2") {
                    output.print("/*" + c.value + "*/");
                    if (start.nlb) {
                        output.print("\n");
                        output.indent();
                    } else {
                        output.space();
                    }
                }
            });
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Node.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.clone"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>clone ()](#apidoc.element.uglifyjs.AST_Node.prototype.clone)
- description and source-code
```javascript
clone = function () {
    return new this.CTOR(this);
}
```
- example usage
```shell
...
    var seq = new AST_Seq(x);
    seq.car = x;
    seq.cdr = y;
    return seq;
},
$from_array: function(array) {
    if (array.length == 0) return null;
    if (array.length == 1) return array[0].clone();
    var list = null;
    for (var i = array.length; --i >= 0;) {
        list = AST_Seq.cons(array[i], list);
    }
    var p = list;
    while (p) {
        if (p.cdr && !p.cdr.cdr) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.equivalent_to"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>equivalent_to (node)](#apidoc.element.uglifyjs.AST_Node.prototype.equivalent_to)
- description and source-code
```javascript
equivalent_to = function (node){
    // XXX: this is a rather expensive way to test two node's equivalence:
    return this.print_to_string() == node.print_to_string();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.evaluate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>evaluate (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.evaluate)
- description and source-code
```javascript
evaluate = function (compressor){
    if (!compressor.option("evaluate")) return [ this ];
    try {
        var val = this._eval(compressor);
        return [ best_of(make_node_from_constant(compressor, val, this), this), val ];
    } catch(ex) {
        if (ex !== def) throw ex;
        return [ this ];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return true }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Node.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){ return false }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>is_string ()](#apidoc.element.uglifyjs.AST_Node.prototype.is_string)
- description and source-code
```javascript
is_string = function (){ return false }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>needs_parens ()](#apidoc.element.uglifyjs.AST_Node.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (){
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Node.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.print"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>print (stream, force_parens)](#apidoc.element.uglifyjs.AST_Node.prototype.print)
- description and source-code
```javascript
print = function (stream, force_parens){
    var self = this, generator = self._codegen;
    function doit() {
        self.add_comments(stream);
        self.add_source_map(stream);
        generator(self, stream);
    }
    stream.push_node(self);
    if (force_parens || self.needs_parens(stream)) {
        stream.with_parens(doit);
    } else {
        doit();
    }
    stream.pop_node();
}
```
- example usage
```shell
...

#### Generating output

AST nodes have a 'print' method that takes an output stream.  Essentially,
to generate code you do this:
'''javascript
var stream = UglifyJS.OutputStream(options);
compressed_ast.print(stream);
var code = stream.toString(); // this is your minified code
'''

or, for a shortcut you can do:
'''javascript
var code = compressed_ast.print_to_string(options);
'''
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.print_to_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>print_to_string (options)](#apidoc.element.uglifyjs.AST_Node.prototype.print_to_string)
- description and source-code
```javascript
print_to_string = function (options){
    var s = OutputStream(options);
    this.print(s);
    return s.get();
}
```
- example usage
```shell
...
var stream = UglifyJS.OutputStream(options);
compressed_ast.print(stream);
var code = stream.toString(); // this is your minified code
'''

or, for a shortcut you can do:
'''javascript
var code = compressed_ast.print_to_string(options);
'''

As usual, 'options' is optional.  The output stream accepts a lot of options,
most of them documented above in section “Beautifier options”.  The two
which we care about here are 'source_map' and 'comments'.

#### Keeping comments in the output
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Node.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```

#### <a name="apidoc.element.uglifyjs.AST_Node.prototype.walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Node.prototype.</span>walk (visitor)](#apidoc.element.uglifyjs.AST_Node.prototype.walk)
- description and source-code
```javascript
walk = function (visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
```
- example usage
```shell
...
    return wrapped_tl;
},
wrap_commonjs: function(name, export_all) {
    var self = this;
    var to_export = [];
    if (export_all) {
        self.figure_out_scope();
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_SymbolDeclaration && node.definition().global) {
                if (!find_if(function(n){ return n.name == node.name }, to_export))
                    to_export.push(node);
            }
        }));
    }
    var wrapped_tl = "(function(exports, global){ global['" + name + "'] = exports; '$ORIG'; '$EXPORTS'; }({}, (function(){return
 this}())))";
...
```



# <a name="apidoc.module.uglifyjs.AST_Null"></a>[module uglifyjs.AST_Null](#apidoc.module.uglifyjs.AST_Null)

#### <a name="apidoc.element.uglifyjs.AST_Null.AST_Null"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Null (props)](#apidoc.element.uglifyjs.AST_Null.AST_Null)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Null.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Null.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Null.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Null.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Null.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Null.prototype"></a>[module uglifyjs.AST_Null.prototype](#apidoc.module.uglifyjs.AST_Null.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Null.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Null.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Null.prototype.CTOR)
- description and source-code
```javascript
function AST_Null(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Null.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Null.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Null.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Number"></a>[module uglifyjs.AST_Number](#apidoc.module.uglifyjs.AST_Number)

#### <a name="apidoc.element.uglifyjs.AST_Number.AST_Number"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Number (props)](#apidoc.element.uglifyjs.AST_Number.AST_Number)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Number.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Number.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Number.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Number.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Number.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Number.prototype"></a>[module uglifyjs.AST_Number.prototype](#apidoc.module.uglifyjs.AST_Number.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Number.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Number.prototype.CTOR)
- description and source-code
```javascript
function AST_Number(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Number.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Number.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print(make_num(self.getValue()));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Number.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Number.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Number.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    if (this.getValue() < 0 && p instanceof AST_PropAccess && p.expression === this)
        return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Object"></a>[module uglifyjs.AST_Object](#apidoc.module.uglifyjs.AST_Object)

#### <a name="apidoc.element.uglifyjs.AST_Object.AST_Object"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Object (props)](#apidoc.element.uglifyjs.AST_Object.AST_Object)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Object.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Object.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Object.prototype"></a>[module uglifyjs.AST_Object.prototype](#apidoc.module.uglifyjs.AST_Object.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Object.prototype.CTOR)
- description and source-code
```javascript
function AST_Object(props){ if (props) { this.end = props.end;this.start = props.start;this.properties = props.properties;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Object.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    if (self.properties.length > 0) output.with_block(function(){
        self.properties.forEach(function(prop, i){
            if (i) {
                output.print(",");
                output.newline();
            }
            output.indent();
            prop.print(output);
        });
        output.newline();
    });
    else output.print("{}");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Object.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.properties.forEach(function(prop){
            prop._walk(visitor);
        });
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Object.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    for (var i = this.properties.length; --i >= 0;)
        if (this.properties[i].has_side_effects(compressor))
            return true;
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Object.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    return first_in_statement(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Object.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Object.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Object.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Object.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Object.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_ObjectGetter"></a>[module uglifyjs.AST_ObjectGetter](#apidoc.module.uglifyjs.AST_ObjectGetter)

#### <a name="apidoc.element.uglifyjs.AST_ObjectGetter.AST_ObjectGetter"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectGetter (props)](#apidoc.element.uglifyjs.AST_ObjectGetter.AST_ObjectGetter)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectGetter.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectGetter.BASE)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectGetter.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectGetter.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectGetter.prototype"></a>[module uglifyjs.AST_ObjectGetter.prototype](#apidoc.module.uglifyjs.AST_ObjectGetter.prototype)

#### <a name="apidoc.element.uglifyjs.AST_ObjectGetter.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectGetter.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectGetter.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectGetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ObjectGetter.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("get");
    output.space();
    self.key.print(output);
    self.value._do_print(output, true);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectKeyVal"></a>[module uglifyjs.AST_ObjectKeyVal](#apidoc.module.uglifyjs.AST_ObjectKeyVal)

#### <a name="apidoc.element.uglifyjs.AST_ObjectKeyVal.AST_ObjectKeyVal"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectKeyVal (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.AST_ObjectKeyVal)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectKeyVal.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.BASE)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectKeyVal.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectKeyVal.prototype"></a>[module uglifyjs.AST_ObjectKeyVal.prototype](#apidoc.module.uglifyjs.AST_ObjectKeyVal.prototype)

#### <a name="apidoc.element.uglifyjs.AST_ObjectKeyVal.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectKeyVal.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectKeyVal.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ObjectKeyVal.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var key = self.key;
    var quote = self.quote;
    if (output.option("quote_keys")) {
        output.print_string(key + "");
    } else if ((typeof key == "number"
                || !output.option("beautify")
                && +key + "" == key)
               && parseFloat(key) >= 0) {
        output.print(make_num(key));
    } else if (RESERVED_WORDS(key) ? output.option("screw_ie8") : is_identifier_string(key)) {
        output.print_name(key);
    } else {
        output.print_string(key, quote);
    }
    output.colon();
    self.value.print(output);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectProperty"></a>[module uglifyjs.AST_ObjectProperty](#apidoc.module.uglifyjs.AST_ObjectProperty)

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.AST_ObjectProperty"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectProperty (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.AST_ObjectProperty)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectProperty.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectProperty.SUBCLASSES"></a>[module uglifyjs.AST_ObjectProperty.SUBCLASSES](#apidoc.module.uglifyjs.AST_ObjectProperty.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.0)
- description and source-code
```javascript
function AST_ObjectKeyVal(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;this.quote = props.quote;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.1)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.SUBCLASSES.2)
- description and source-code
```javascript
function AST_ObjectGetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectProperty.prototype"></a>[module uglifyjs.AST_ObjectProperty.prototype](#apidoc.module.uglifyjs.AST_ObjectProperty.prototype)

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.value._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.value.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectProperty.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectProperty.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_ObjectProperty.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_ObjectSetter"></a>[module uglifyjs.AST_ObjectSetter](#apidoc.module.uglifyjs.AST_ObjectSetter)

#### <a name="apidoc.element.uglifyjs.AST_ObjectSetter.AST_ObjectSetter"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_ObjectSetter (props)](#apidoc.element.uglifyjs.AST_ObjectSetter.AST_ObjectSetter)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectSetter.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>BASE (props)](#apidoc.element.uglifyjs.AST_ObjectSetter.BASE)
- description and source-code
```javascript
function AST_ObjectProperty(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key
 = props.key;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectSetter.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_ObjectSetter.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_ObjectSetter.prototype"></a>[module uglifyjs.AST_ObjectSetter.prototype](#apidoc.module.uglifyjs.AST_ObjectSetter.prototype)

#### <a name="apidoc.element.uglifyjs.AST_ObjectSetter.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_ObjectSetter.prototype.CTOR)
- description and source-code
```javascript
function AST_ObjectSetter(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.key =
props.key;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_ObjectSetter.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_ObjectSetter.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_ObjectSetter.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("set");
    output.space();
    self.key.print(output);
    self.value._do_print(output, true);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_PropAccess"></a>[module uglifyjs.AST_PropAccess](#apidoc.module.uglifyjs.AST_PropAccess)

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.AST_PropAccess"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_PropAccess (props)](#apidoc.element.uglifyjs.AST_PropAccess.AST_PropAccess)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>BASE (props)](#apidoc.element.uglifyjs.AST_PropAccess.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_PropAccess.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_PropAccess.SUBCLASSES"></a>[module uglifyjs.AST_PropAccess.SUBCLASSES](#apidoc.module.uglifyjs.AST_PropAccess.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_PropAccess.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Dot(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_PropAccess.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_PropAccess.prototype"></a>[module uglifyjs.AST_PropAccess.prototype](#apidoc.module.uglifyjs.AST_PropAccess.prototype)

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_PropAccess.prototype.CTOR)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_PropAccess.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return !compressor.option("pure_getters");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_PropAccess.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    if (p instanceof AST_New && p.expression === this) {
        // i.e. new (foo.bar().baz)
        //
        // if there's one call into this subtree, then we need
        // parens around it too, otherwise the call will be
        // interpreted as passing the arguments to the upper New
        // expression.
        try {
            this.walk(new TreeWalker(function(node){
                if (node instanceof AST_Call) throw p;
            }));
        } catch(ex) {
            if (ex !== p) throw ex;
            return true;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_PropAccess.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_PropAccess.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_PropAccess.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_RegExp"></a>[module uglifyjs.AST_RegExp](#apidoc.module.uglifyjs.AST_RegExp)

#### <a name="apidoc.element.uglifyjs.AST_RegExp.AST_RegExp"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_RegExp (props)](#apidoc.element.uglifyjs.AST_RegExp.AST_RegExp)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_RegExp.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>BASE (props)](#apidoc.element.uglifyjs.AST_RegExp.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_RegExp.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_RegExp.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_RegExp.prototype"></a>[module uglifyjs.AST_RegExp.prototype](#apidoc.module.uglifyjs.AST_RegExp.prototype)

#### <a name="apidoc.element.uglifyjs.AST_RegExp.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_RegExp.prototype.CTOR)
- description and source-code
```javascript
function AST_RegExp(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_RegExp.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_RegExp.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var str = self.getValue().toString();
    if (output.option("ascii_only")) {
        str = output.to_ascii(str);
    } else if (output.option("unescape_regexps")) {
        str = str.split("\\\\").map(function(str){
            return str.replace(/\\u[0-9a-fA-F]{4}|\\x[0-9a-fA-F]{2}/g, function(s){
                var code = parseInt(s.substr(2), 16);
                return regexp_safe_literal(code) ? String.fromCharCode(code) : s;
            });
        }).join("\\\\");
    }
    output.print(str);
    var p = output.parent();
    if (p instanceof AST_Binary && /^in/.test(p.operator) && p.left === self)
        output.print(" ");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_RegExp.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_RegExp.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_RegExp.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Return"></a>[module uglifyjs.AST_Return](#apidoc.module.uglifyjs.AST_Return)

#### <a name="apidoc.element.uglifyjs.AST_Return.AST_Return"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Return (props)](#apidoc.element.uglifyjs.AST_Return.AST_Return)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Return.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Return.BASE)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Return.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Return.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Return.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Return.prototype"></a>[module uglifyjs.AST_Return.prototype](#apidoc.module.uglifyjs.AST_Return.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Return.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Return.prototype.CTOR)
- description and source-code
```javascript
function AST_Return(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Return.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Return.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "return");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Return.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Return.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Return.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Scope"></a>[module uglifyjs.AST_Scope](#apidoc.module.uglifyjs.AST_Scope)

#### <a name="apidoc.element.uglifyjs.AST_Scope.AST_Scope"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Scope (props)](#apidoc.element.uglifyjs.AST_Scope.AST_Scope)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Scope.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Scope.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Scope.SUBCLASSES"></a>[module uglifyjs.AST_Scope.SUBCLASSES](#apidoc.module.uglifyjs.AST_Scope.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Scope.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Scope.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Scope.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Lambda(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.uses_arguments
 = props.uses_arguments;this.argnames = props.argnames;this.name = props.name;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Scope.prototype"></a>[module uglifyjs.AST_Scope.prototype](#apidoc.module.uglifyjs.AST_Scope.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Scope.prototype.CTOR)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.def_function"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>def_function (symbol)](#apidoc.element.uglifyjs.AST_Scope.prototype.def_function)
- description and source-code
```javascript
def_function = function (symbol){
    this.functions.set(symbol.name, this.def_variable(symbol));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.def_variable"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>def_variable (symbol)](#apidoc.element.uglifyjs.AST_Scope.prototype.def_variable)
- description and source-code
```javascript
def_variable = function (symbol){
    var def;
    if (!this.variables.has(symbol.name)) {
        def = new SymbolDef(this, this.variables.size(), symbol);
        this.variables.set(symbol.name, def);
        def.global = !this.parent_scope;
    } else {
        def = this.variables.get(symbol.name);
        def.orig.push(symbol);
    }
    return symbol.thedef = def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.drop_unused"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>drop_unused (compressor)](#apidoc.element.uglifyjs.AST_Scope.prototype.drop_unused)
- description and source-code
```javascript
drop_unused = function (compressor){
    var self = this;
    if (compressor.option("unused")
        && !(self instanceof AST_Toplevel)
        && !self.uses_eval
       ) {
        var in_use = [];
        var initializations = new Dictionary();
        // pass 1: find out which symbols are directly used in
        // this scope (not in nested scopes).
        var scope = this;
        var tw = new TreeWalker(function(node, descend){
            if (node !== self) {
                if (node instanceof AST_Defun) {
                    initializations.add(node.name.name, node);
                    return true; // don't go in nested scopes
                }
                if (node instanceof AST_Definitions && scope === self) {
                    node.definitions.forEach(function(def){
                        if (def.value) {
                            initializations.add(def.name.name, def.value);
                            if (def.value.has_side_effects(compressor)) {
                                def.value.walk(tw);
                            }
                        }
                    });
                    return true;
                }
                if (node instanceof AST_SymbolRef) {
                    push_uniq(in_use, node.definition());
                    return true;
                }
                if (node instanceof AST_Scope) {
                    var save_scope = scope;
                    scope = node;
                    descend();
                    scope = save_scope;
                    return true;
                }
            }
        });
        self.walk(tw);
        // pass 2: for every used symbol we need to walk its
        // initialization code to figure out if it uses other
        // symbols (that may not be in_use).
        for (var i = 0; i < in_use.length; ++i) {
            in_use[i].orig.forEach(function(decl){
                // undeclared globals will be instanceof AST_SymbolRef
                var init = initializations.get(decl.name);
                if (init) init.forEach(function(init){
                    var tw = new TreeWalker(function(node){
                        if (node instanceof AST_SymbolRef) {
                            push_uniq(in_use, node.definition());
                        }
                    });
                    init.walk(tw);
                });
            });
        }
        // pass 3: we should drop declarations not in_use
        var tt = new TreeTransformer(
            function before(node, descend, in_list) {
                if (node instanceof AST_Lambda && !(node instanceof AST_Accessor)) {
                    if (!compressor.option("keep_fargs")) {
                        for (var a = node.argnames, i = a.length; --i >= 0;) {
                            var sym = a[i];
                            if (sym.unreferenced()) {
                                a.pop();
                                compressor.warn("Dropping unused function argument {name} [{file}:{line},{col}]", {
                                    name : sym.name,
                                    file : sym.start.file,
                                    line : sym.start.line,
                                    col  : sym.start.col
                                });
                            }
                            else break;
                        }
                    }
                }
                if (node instanceof AST_Defun && node !== self) {
                    if (!member(node.name.definition(), in_use)) {
                        compressor.warn("Dropping unused function {name} [{file}:{line},{col}]", {
                            name : node.name.name,
                            file : node.name.start.file,
                            line : node.name.start.line,
                            col  : node.name.start.col
                        });
                        return make_node(AST_EmptyStatement, node);
                    }
                    return node;
                }
                if (node instanceof AST_Definitions && !( ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.find_variable"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>find_variable (name)](#apidoc.element.uglifyjs.AST_Scope.prototype.find_variable)
- description and source-code
```javascript
find_variable = function (name){
    if (name instanceof AST_Symbol) name = name.name;
    return this.variables.get(name)
        || (this.parent_scope && this.parent_scope.find_variable(name));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.has_directive"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>has_directive (value)](#apidoc.element.uglifyjs.AST_Scope.prototype.has_directive)
- description and source-code
```javascript
has_directive = function (value){
    return this.parent_scope && this.parent_scope.has_directive(value)
        || (this.directives.indexOf(value) >= 0 ? this : null);
}
```
- example usage
```shell
...
    var stack = this.stack;
    for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof type) return x;
    }
},
has_directive: function(type) {
    return this.find_parent(AST_Scope).has_directive(type);
},
in_boolean_context: function() {
    var stack = this.stack;
    var i = stack.length, self = stack[--i];
    while (i > 0) {
        var p = stack[--i];
        if ((p instanceof AST_If           && p.condition === self) ||
...
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.hoist_declarations"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>hoist_declarations (compressor)](#apidoc.element.uglifyjs.AST_Scope.prototype.hoist_declarations)
- description and source-code
```javascript
hoist_declarations = function (compressor){
    var hoist_funs = compressor.option("hoist_funs");
    var hoist_vars = compressor.option("hoist_vars");
    var self = this;
    if (hoist_funs || hoist_vars) {
        var dirs = [];
        var hoisted = [];
        var vars = new Dictionary(), vars_found = 0, var_decl = 0;
        // let's count var_decl first, we seem to waste a lot of
        // space if we hoist 'var' when there's only one.
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_Scope && node !== self)
                return true;
            if (node instanceof AST_Var) {
                ++var_decl;
                return true;
            }
        }));
        hoist_vars = hoist_vars && var_decl > 1;
        var tt = new TreeTransformer(
            function before(node) {
                if (node !== self) {
                    if (node instanceof AST_Directive) {
                        dirs.push(node);
                        return make_node(AST_EmptyStatement, node);
                    }
                    if (node instanceof AST_Defun && hoist_funs) {
                        hoisted.push(node);
                        return make_node(AST_EmptyStatement, node);
                    }
                    if (node instanceof AST_Var && hoist_vars) {
                        node.definitions.forEach(function(def){
                            vars.set(def.name.name, def);
                            ++vars_found;
                        });
                        var seq = node.to_assignments();
                        var p = tt.parent();
                        if (p instanceof AST_ForIn && p.init === node) {
                            if (seq == null) return node.definitions[0].name;
                            return seq;
                        }
                        if (p instanceof AST_For && p.init === node) {
                            return seq;
                        }
                        if (!seq) return make_node(AST_EmptyStatement, node);
                        return make_node(AST_SimpleStatement, node, {
                            body: seq
                        });
                    }
                    if (node instanceof AST_Scope)
                        return node; // to avoid descending in nested scopes
                }
            }
        );
        self = self.transform(tt);
        if (vars_found > 0) {
            // collect only vars which don't show up in self's arguments list
            var defs = [];
            vars.each(function(def, name){
                if (self instanceof AST_Lambda
                    && find_if(function(x){ return x.name == def.name.name },
                               self.argnames)) {
                    vars.del(name);
                } else {
                    def = def.clone();
                    def.value = null;
                    defs.push(def);
                    vars.set(name, def);
                }
            });
            if (defs.length > 0) {
                // try to merge in assignments
                for (var i = 0; i < self.body.length;) {
                    if (self.body[i] instanceof AST_SimpleStatement) {
                        var expr = self.body[i].body, sym, assign;
                        if (expr instanceof AST_Assign
                            && expr.operator == "="
                            && (sym = expr.left) instanceof AST_Symbol
                            && vars.has(sym.name))
                        {
                            var def = vars.get(sym.name);
                            if (def.value) break;
                            def.value = expr.right;
                            remove(defs, def);
                            defs.push(def);
                            self.body.splice(i, 1);
                            continue;
                        }
                        if (expr instanceof AST_Seq
                            && (assign = expr.car) instanceof AST_Assign
                            && assign.operator == "=" ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.init_scope_vars"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>init_scope_vars (nesting)](#apidoc.element.uglifyjs.AST_Scope.prototype.init_scope_vars)
- description and source-code
```javascript
init_scope_vars = function (nesting){
    this.directives = [];     // contains the directives defined in this scope, i.e. "use strict"
    this.variables = new Dictionary(); // map name to AST_SymbolVar (variables defined in this scope; includes functions)
    this.functions = new Dictionary(); // map name to AST_SymbolDefun (functions defined in this scope)
    this.uses_with = false;   // will be set to true if this or some nested scope uses the 'with' statement
    this.uses_eval = false;   // will be set to true if this or nested scope uses the global 'eval'
    this.parent_scope = null; // the parent scope
    this.enclosed = [];       // a list of variables from this or outer scope(s) that are referenced from this or inner scopes
    this.cname = -1;          // the current index for mangling functions/variables
    this.nesting = nesting;   // the nesting level of this scope (0 means toplevel)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.next_mangled"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>next_mangled (options)](#apidoc.element.uglifyjs.AST_Scope.prototype.next_mangled)
- description and source-code
```javascript
next_mangled = function (options){
    var ext = this.enclosed;
    out: while (true) {
        var m = base54(++this.cname);
        if (!is_identifier(m)) continue; // skip over "do"

        // https://github.com/mishoo/UglifyJS2/issues/242 -- do not
        // shadow a name excepted from mangling.
        if (options.except.indexOf(m) >= 0) continue;

        // we must ensure that the mangled name does not shadow a name
        // from some parent scope that is referenced in this or in
        // inner scopes.
        for (var i = ext.length; --i >= 0;) {
            var sym = ext[i];
            var name = sym.mangled_name || (sym.unmangleable(options) && sym.name);
            if (m == name) continue out;
        }
        return m;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.references"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>references (sym)](#apidoc.element.uglifyjs.AST_Scope.prototype.references)
- description and source-code
```javascript
references = function (sym){
    if (sym instanceof AST_Symbol) sym = sym.definition();
    return this.enclosed.indexOf(sym) < 0 ? null : sym;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Scope.prototype.strict"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Scope.prototype.</span>strict ()](#apidoc.element.uglifyjs.AST_Scope.prototype.strict)
- description and source-code
```javascript
strict = function (){
    return this.has_directive("use strict");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Seq"></a>[module uglifyjs.AST_Seq](#apidoc.module.uglifyjs.AST_Seq)

#### <a name="apidoc.element.uglifyjs.AST_Seq.AST_Seq"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Seq (props)](#apidoc.element.uglifyjs.AST_Seq.AST_Seq)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Seq.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Seq.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.cons"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>cons (x, y)](#apidoc.element.uglifyjs.AST_Seq.cons)
- description and source-code
```javascript
cons = function (x, y) {
    var seq = new AST_Seq(x);
    seq.car = x;
    seq.cdr = y;
    return seq;
}
```
- example usage
```shell
...
    return seq;
},
$from_array: function(array) {
    if (array.length == 0) return null;
    if (array.length == 1) return array[0].clone();
    var list = null;
    for (var i = array.length; --i >= 0;) {
        list = AST_Seq.cons(array[i], list);
    }
    var p = list;
    while (p) {
        if (p.cdr && !p.cdr.cdr) {
            p.cdr = p.cdr.car;
            break;
        }
...
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.from_array"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.</span>from_array (array)](#apidoc.element.uglifyjs.AST_Seq.from_array)
- description and source-code
```javascript
from_array = function (array) {
    if (array.length == 0) return null;
    if (array.length == 1) return array[0].clone();
    var list = null;
    for (var i = array.length; --i >= 0;) {
        list = AST_Seq.cons(array[i], list);
    }
    var p = list;
    while (p) {
        if (p.cdr && !p.cdr.cdr) {
            p.cdr = p.cdr.car;
            break;
        }
        p = p.cdr;
    }
    return list;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Seq.prototype"></a>[module uglifyjs.AST_Seq.prototype](#apidoc.module.uglifyjs.AST_Seq.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Seq.prototype.CTOR)
- description and source-code
```javascript
function AST_Seq(props){ if (props) { this.end = props.end;this.start = props.start;this.cdr = props.cdr;this.car = props.car;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Seq.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output);
    // var p = output.parent();
    // if (p instanceof AST_Statement) {
    //     output.with_indent(output.next_indent(), function(){
    //         self._do_print(output);
    //     });
    // } else {
    //     self._do_print(output);
    // }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype._do_print"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>_do_print (output)](#apidoc.element.uglifyjs.AST_Seq.prototype._do_print)
- description and source-code
```javascript
_do_print = function (output){
    this.car.print(output);
    if (this.cdr) {
        output.comma();
        if (output.should_break()) {
            output.newline();
            output.indent();
        }
        this.cdr.print(output);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Seq.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.car._walk(visitor);
        if (this.cdr) this.cdr._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.add"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>add (node)](#apidoc.element.uglifyjs.AST_Seq.prototype.add)
- description and source-code
```javascript
add = function (node) {
    var p = this;
    while (p) {
        if (!(p.cdr instanceof AST_Seq)) {
            var cell = AST_Seq.cons(p.cdr, node);
            return p.cdr = cell;
        }
        p = p.cdr;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.car.has_side_effects(compressor)
        || this.cdr.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_Seq.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return this.cdr.is_boolean();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>is_string (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.is_string)
- description and source-code
```javascript
is_string = function (compressor){
    return this.cdr.is_string(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Seq.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    return p instanceof AST_Call             // (foo, bar)() or foo(1, (2, 3), 4)
        || p instanceof AST_Unary            // !(foo, bar, baz)
        || p instanceof AST_Binary           // 1 + (2, 3) + 4 ==> 8
        || p instanceof AST_VarDef           // var a = (1, 2), b = a + a; ==> b == 4
        || p instanceof AST_PropAccess       // (1, {foo:2}).foo or (1, {foo:2})["foo"] ==> 2
        || p instanceof AST_Array            // [ 1, (2, 3), 4 ] ==> [ 1, 3, 4 ]
        || p instanceof AST_ObjectProperty   // { foo: (1, 2) }.foo ==> 2
        || p instanceof AST_Conditional<span class="apidocCodeCommentSpan">      /* (false, true) ? (a = 10, b = 20) : (c = 30)
                                              * ==> 20 (side effect, set a := 10 and b := 20) */
</span>    ;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Seq.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.to_array"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>to_array ()](#apidoc.element.uglifyjs.AST_Seq.prototype.to_array)
- description and source-code
```javascript
to_array = function () {
    var p = this, a = [];
    while (p) {
        a.push(p.car);
        if (p.cdr && !(p.cdr instanceof AST_Seq)) {
            a.push(p.cdr);
            break;
        }
        p = p.cdr;
    }
    return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Seq.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Seq.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Seq.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Seq.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_SimpleStatement"></a>[module uglifyjs.AST_SimpleStatement](#apidoc.module.uglifyjs.AST_SimpleStatement)

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.AST_SimpleStatement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SimpleStatement (props)](#apidoc.element.uglifyjs.AST_SimpleStatement.AST_SimpleStatement)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SimpleStatement.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SimpleStatement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SimpleStatement.prototype"></a>[module uglifyjs.AST_SimpleStatement.prototype](#apidoc.module.uglifyjs.AST_SimpleStatement.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.CTOR)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.body.print(output);
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.body.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_SimpleStatement.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SimpleStatement.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_SimpleStatement.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Statement"></a>[module uglifyjs.AST_Statement](#apidoc.module.uglifyjs.AST_Statement)

#### <a name="apidoc.element.uglifyjs.AST_Statement.AST_Statement"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Statement (props)](#apidoc.element.uglifyjs.AST_Statement.AST_Statement)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Statement.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Statement.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Statement.SUBCLASSES"></a>[module uglifyjs.AST_Statement.SUBCLASSES](#apidoc.module.uglifyjs.AST_Statement.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Debugger(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Directive(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.scope =
props.scope;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.2)
- description and source-code
```javascript
function AST_SimpleStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.3)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.4)
- description and source-code
```javascript
function AST_EmptyStatement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.5)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.6"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>6 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.6)
- description and source-code
```javascript
function AST_Jump(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.7"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.SUBCLASSES.</span>7 (props)](#apidoc.element.uglifyjs.AST_Statement.SUBCLASSES.7)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Statement.prototype"></a>[module uglifyjs.AST_Statement.prototype](#apidoc.module.uglifyjs.AST_Statement.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Statement.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Statement.prototype.CTOR)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Statement.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.body.print(output);
    output.semicolon();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>_eval ()](#apidoc.element.uglifyjs.AST_Statement.prototype._eval)
- description and source-code
```javascript
_eval = function (){
    throw new Error(string_template("Cannot evaluate a statement [{file}:{line},{col}]", this.start));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_Statement.prototype.aborts)
- description and source-code
```javascript
aborts = function (){ return null }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Statement.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Statement.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_Statement.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_StatementWithBody"></a>[module uglifyjs.AST_StatementWithBody](#apidoc.module.uglifyjs.AST_StatementWithBody)

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.AST_StatementWithBody"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_StatementWithBody (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.AST_StatementWithBody)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>BASE (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.BASE)
- description and source-code
```javascript
function AST_Statement(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_StatementWithBody.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_StatementWithBody.SUBCLASSES"></a>[module uglifyjs.AST_StatementWithBody.SUBCLASSES](#apidoc.module.uglifyjs.AST_StatementWithBody.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.0)
- description and source-code
```javascript
function AST_LabeledStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.label
 = props.label;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.1)
- description and source-code
```javascript
function AST_IterationStatement(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.2)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.SUBCLASSES.3)
- description and source-code
```javascript
function AST_If(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.alternative = props
.alternative;this.condition = props.condition;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_StatementWithBody.prototype"></a>[module uglifyjs.AST_StatementWithBody.prototype](#apidoc.module.uglifyjs.AST_StatementWithBody.prototype)

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype.CTOR)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.prototype._do_print_body"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>_do_print_body (output)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype._do_print_body)
- description and source-code
```javascript
_do_print_body = function (output){
    force_statement(this.body, output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_StatementWithBody.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_StatementWithBody.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_StatementWithBody.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_String"></a>[module uglifyjs.AST_String](#apidoc.module.uglifyjs.AST_String)

#### <a name="apidoc.element.uglifyjs.AST_String.AST_String"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_String (props)](#apidoc.element.uglifyjs.AST_String.AST_String)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_String.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>BASE (props)](#apidoc.element.uglifyjs.AST_String.BASE)
- description and source-code
```javascript
function AST_Constant(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_String.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_String.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_String.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_String.prototype"></a>[module uglifyjs.AST_String.prototype](#apidoc.module.uglifyjs.AST_String.prototype)

#### <a name="apidoc.element.uglifyjs.AST_String.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_String.prototype.CTOR)
- description and source-code
```javascript
function AST_String(props){ if (props) { this.end = props.end;this.start = props.start;this.quote = props.quote;this.value = props
.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_String.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_String.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print_string(self.getValue(), self.quote);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_String.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_String.prototype.</span>is_string ()](#apidoc.element.uglifyjs.AST_String.prototype.is_string)
- description and source-code
```javascript
is_string = function (){ return true }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Sub"></a>[module uglifyjs.AST_Sub](#apidoc.module.uglifyjs.AST_Sub)

#### <a name="apidoc.element.uglifyjs.AST_Sub.AST_Sub"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Sub (props)](#apidoc.element.uglifyjs.AST_Sub.AST_Sub)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Sub.BASE)
- description and source-code
```javascript
function AST_PropAccess(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Sub.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Sub.prototype"></a>[module uglifyjs.AST_Sub.prototype](#apidoc.module.uglifyjs.AST_Sub.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Sub.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Sub.prototype.CTOR)
- description and source-code
```javascript
function AST_Sub(props){ if (props) { this.end = props.end;this.start = props.start;this.property = props.property;this.expression
 = props.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Sub.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.expression.print(output);
    output.print("[");
    self.property.print(output);
    output.print("]");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Sub.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        this.property._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Sub.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    if (!compressor.option("pure_getters")) return true;
    return this.expression.has_side_effects(compressor)
        || this.property.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Sub.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Sub.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Sub.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Sub.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Switch"></a>[module uglifyjs.AST_Switch](#apidoc.module.uglifyjs.AST_Switch)

#### <a name="apidoc.element.uglifyjs.AST_Switch.AST_Switch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Switch (props)](#apidoc.element.uglifyjs.AST_Switch.AST_Switch)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Switch.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Switch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Switch.prototype"></a>[module uglifyjs.AST_Switch.prototype](#apidoc.module.uglifyjs.AST_Switch.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Switch.prototype.CTOR)
- description and source-code
```javascript
function AST_Switch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression =
props.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Switch.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("switch");
    output.space();
    output.with_parens(function(){
        self.expression.print(output);
    });
    output.space();
    if (self.body.length > 0) output.with_block(function(){
        self.body.forEach(function(stmt, i){
            if (i) output.newline();
            output.indent(true);
            stmt.print(output);
        });
    });
    else output.print("{}");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Switch.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        walk_body(this, visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Switch.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Switch.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Switch.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Switch.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Switch.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Switch.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_SwitchBranch"></a>[module uglifyjs.AST_SwitchBranch](#apidoc.module.uglifyjs.AST_SwitchBranch)

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.AST_SwitchBranch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SwitchBranch (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.AST_SwitchBranch)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SwitchBranch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SwitchBranch.SUBCLASSES"></a>[module uglifyjs.AST_SwitchBranch.SUBCLASSES](#apidoc.module.uglifyjs.AST_SwitchBranch.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.SUBCLASSES.0)
- description and source-code
```javascript
function AST_Default(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.SUBCLASSES.1)
- description and source-code
```javascript
function AST_Case(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SwitchBranch.prototype"></a>[module uglifyjs.AST_SwitchBranch.prototype](#apidoc.module.uglifyjs.AST_SwitchBranch.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.CTOR)
- description and source-code
```javascript
function AST_SwitchBranch(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.prototype._do_print_body"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>_do_print_body (output)](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype._do_print_body)
- description and source-code
```javascript
_do_print_body = function (output){
    if (this.body.length > 0) {
        output.newline();
        this.body.forEach(function(stmt){
            output.indent();
            stmt.print(output);
            output.newline();
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.prototype.aborts"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>aborts ()](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.aborts)
- description and source-code
```javascript
function block_aborts(){
    var n = this.body.length;
    return n > 0 && aborts(this.body[n - 1]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SwitchBranch.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SwitchBranch.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_SwitchBranch.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Symbol"></a>[module uglifyjs.AST_Symbol](#apidoc.module.uglifyjs.AST_Symbol)

#### <a name="apidoc.element.uglifyjs.AST_Symbol.AST_Symbol"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Symbol (props)](#apidoc.element.uglifyjs.AST_Symbol.AST_Symbol)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Symbol.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Symbol.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Symbol.SUBCLASSES"></a>[module uglifyjs.AST_Symbol.SUBCLASSES](#apidoc.module.uglifyjs.AST_Symbol.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.0)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.1)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.2)
- description and source-code
```javascript
function AST_Label(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;this.references = props.references;this.initialize();}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.3)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.4)
- description and source-code
```javascript
function AST_LabelRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.5"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.SUBCLASSES.</span>5 (props)](#apidoc.element.uglifyjs.AST_Symbol.SUBCLASSES.5)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Symbol.prototype"></a>[module uglifyjs.AST_Symbol.prototype](#apidoc.module.uglifyjs.AST_Symbol.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Symbol.prototype.CTOR)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Symbol.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var def = self.definition();
    output.print_name(def ? def.mangled_name || def.name : self.name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Symbol.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.definition"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>definition ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.definition)
- description and source-code
```javascript
definition = function (){
    return this.thedef;
}
```
- example usage
```shell
...
},
wrap_commonjs: function(name, export_all) {
    var self = this;
    var to_export = [];
    if (export_all) {
        self.figure_out_scope();
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_SymbolDeclaration && node.definition().global) {
                if (!find_if(function(n){ return n.name == node.name }, to_export))
                    to_export.push(node);
            }
        }));
    }
    var wrapped_tl = "(function(exports, global){ global['" + name + "'] = exports; '$ORIG'; '$EXPORTS'; }({}, (function(){return
 this}())))";
    wrapped_tl = parse(wrapped_tl);
...
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.global"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>global ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.global)
- description and source-code
```javascript
global = function (){
    return this.definition().global;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.undeclared"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>undeclared ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.undeclared)
- description and source-code
```javascript
undeclared = function (){
    return this.definition().undeclared;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>unmangleable (options)](#apidoc.element.uglifyjs.AST_Symbol.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (options){
    return this.definition().unmangleable(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Symbol.prototype.unreferenced"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Symbol.prototype.</span>unreferenced ()](#apidoc.element.uglifyjs.AST_Symbol.prototype.unreferenced)
- description and source-code
```javascript
unreferenced = function (){
    return this.definition().references.length == 0
        && !(this.scope.uses_eval || this.scope.uses_with);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolAccessor"></a>[module uglifyjs.AST_SymbolAccessor](#apidoc.module.uglifyjs.AST_SymbolAccessor)

#### <a name="apidoc.element.uglifyjs.AST_SymbolAccessor.AST_SymbolAccessor"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolAccessor (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor.AST_SymbolAccessor)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolAccessor.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolAccessor.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolAccessor.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolAccessor.prototype"></a>[module uglifyjs.AST_SymbolAccessor.prototype](#apidoc.module.uglifyjs.AST_SymbolAccessor.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolAccessor.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolAccessor.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolAccessor(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolAccessor.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolAccessor.prototype.</span>unmangleable ()](#apidoc.element.uglifyjs.AST_SymbolAccessor.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (){
    return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolCatch"></a>[module uglifyjs.AST_SymbolCatch](#apidoc.module.uglifyjs.AST_SymbolCatch)

#### <a name="apidoc.element.uglifyjs.AST_SymbolCatch.AST_SymbolCatch"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolCatch (props)](#apidoc.element.uglifyjs.AST_SymbolCatch.AST_SymbolCatch)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolCatch.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolCatch.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolCatch.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolCatch.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolCatch.prototype"></a>[module uglifyjs.AST_SymbolCatch.prototype](#apidoc.module.uglifyjs.AST_SymbolCatch.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolCatch.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolCatch.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolCatch.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_SymbolConst"></a>[module uglifyjs.AST_SymbolConst](#apidoc.module.uglifyjs.AST_SymbolConst)

#### <a name="apidoc.element.uglifyjs.AST_SymbolConst.AST_SymbolConst"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolConst (props)](#apidoc.element.uglifyjs.AST_SymbolConst.AST_SymbolConst)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolConst.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolConst.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolConst.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolConst.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolConst.prototype"></a>[module uglifyjs.AST_SymbolConst.prototype](#apidoc.module.uglifyjs.AST_SymbolConst.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolConst.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolConst.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolConst.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_SymbolDeclaration"></a>[module uglifyjs.AST_SymbolDeclaration](#apidoc.module.uglifyjs.AST_SymbolDeclaration)

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.AST_SymbolDeclaration"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDeclaration (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.AST_SymbolDeclaration)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolDeclaration.SUBCLASSES"></a>[module uglifyjs.AST_SymbolDeclaration.SUBCLASSES](#apidoc.module.uglifyjs.AST_SymbolDeclaration.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.0)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.1)
- description and source-code
```javascript
function AST_SymbolConst(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.2"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>2 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.2)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.3"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>3 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.3)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.4"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.SUBCLASSES.</span>4 (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.SUBCLASSES.4)
- description and source-code
```javascript
function AST_SymbolCatch(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolDeclaration.prototype"></a>[module uglifyjs.AST_SymbolDeclaration.prototype](#apidoc.module.uglifyjs.AST_SymbolDeclaration.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolDeclaration.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDeclaration.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolDeclaration.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_SymbolDefun"></a>[module uglifyjs.AST_SymbolDefun](#apidoc.module.uglifyjs.AST_SymbolDefun)

#### <a name="apidoc.element.uglifyjs.AST_SymbolDefun.AST_SymbolDefun"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolDefun (props)](#apidoc.element.uglifyjs.AST_SymbolDefun.AST_SymbolDefun)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDefun.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolDefun.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolDefun.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolDefun.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolDefun.prototype"></a>[module uglifyjs.AST_SymbolDefun.prototype](#apidoc.module.uglifyjs.AST_SymbolDefun.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolDefun.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolDefun.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolDefun.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolDefun(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_SymbolFunarg"></a>[module uglifyjs.AST_SymbolFunarg](#apidoc.module.uglifyjs.AST_SymbolFunarg)

#### <a name="apidoc.element.uglifyjs.AST_SymbolFunarg.AST_SymbolFunarg"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolFunarg (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg.AST_SymbolFunarg)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolFunarg.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg.BASE)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolFunarg.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolFunarg.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolFunarg.prototype"></a>[module uglifyjs.AST_SymbolFunarg.prototype](#apidoc.module.uglifyjs.AST_SymbolFunarg.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolFunarg.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolFunarg.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolFunarg.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_SymbolLambda"></a>[module uglifyjs.AST_SymbolLambda](#apidoc.module.uglifyjs.AST_SymbolLambda)

#### <a name="apidoc.element.uglifyjs.AST_SymbolLambda.AST_SymbolLambda"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolLambda (props)](#apidoc.element.uglifyjs.AST_SymbolLambda.AST_SymbolLambda)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolLambda.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolLambda.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolLambda.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolLambda.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolLambda.prototype"></a>[module uglifyjs.AST_SymbolLambda.prototype](#apidoc.module.uglifyjs.AST_SymbolLambda.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolLambda.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolLambda.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolLambda.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolLambda(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_SymbolRef"></a>[module uglifyjs.AST_SymbolRef](#apidoc.module.uglifyjs.AST_SymbolRef)

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.AST_SymbolRef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolRef (props)](#apidoc.element.uglifyjs.AST_SymbolRef.AST_SymbolRef)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolRef.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolRef.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolRef.prototype"></a>[module uglifyjs.AST_SymbolRef.prototype](#apidoc.module.uglifyjs.AST_SymbolRef.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolRef(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    var d = this.definition();
    if (d && d.constant && d.init) return ev(d.init, compressor);
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.global() && this.undeclared();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolRef.prototype.reference"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolRef.prototype.</span>reference ()](#apidoc.element.uglifyjs.AST_SymbolRef.prototype.reference)
- description and source-code
```javascript
reference = function () {
    var def = this.definition();
    def.references.push(this);
    var s = this.scope;
    while (s) {
        push_uniq(s.enclosed, def);
        if (s === def.scope) break;
        s = s.parent_scope;
    }
    this.frame = this.scope.nesting - def.scope.nesting;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolVar"></a>[module uglifyjs.AST_SymbolVar](#apidoc.module.uglifyjs.AST_SymbolVar)

#### <a name="apidoc.element.uglifyjs.AST_SymbolVar.AST_SymbolVar"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_SymbolVar (props)](#apidoc.element.uglifyjs.AST_SymbolVar.AST_SymbolVar)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolVar.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>BASE (props)](#apidoc.element.uglifyjs.AST_SymbolVar.BASE)
- description and source-code
```javascript
function AST_SymbolDeclaration(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this
.name = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_SymbolVar.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_SymbolVar.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolVar.SUBCLASSES"></a>[module uglifyjs.AST_SymbolVar.SUBCLASSES](#apidoc.module.uglifyjs.AST_SymbolVar.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_SymbolVar.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_SymbolVar.SUBCLASSES.0)
- description and source-code
```javascript
function AST_SymbolFunarg(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name
 = props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_SymbolVar.prototype"></a>[module uglifyjs.AST_SymbolVar.prototype](#apidoc.module.uglifyjs.AST_SymbolVar.prototype)

#### <a name="apidoc.element.uglifyjs.AST_SymbolVar.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_SymbolVar.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_SymbolVar.prototype.CTOR)
- description and source-code
```javascript
function AST_SymbolVar(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name =
props.name;this.scope = props.scope;this.init = props.init;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_This"></a>[module uglifyjs.AST_This](#apidoc.module.uglifyjs.AST_This)

#### <a name="apidoc.element.uglifyjs.AST_This.AST_This"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_This (props)](#apidoc.element.uglifyjs.AST_This.AST_This)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_This.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>BASE (props)](#apidoc.element.uglifyjs.AST_This.BASE)
- description and source-code
```javascript
function AST_Symbol(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_This.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_This.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_This.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_This.prototype"></a>[module uglifyjs.AST_This.prototype](#apidoc.module.uglifyjs.AST_This.prototype)

#### <a name="apidoc.element.uglifyjs.AST_This.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_This.prototype.CTOR)
- description and source-code
```javascript
function AST_This(props){ if (props) { this.end = props.end;this.start = props.start;this.thedef = props.thedef;this.name = props
.name;this.scope = props.scope;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_This.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_This.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("this");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_This.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_This.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){ return false }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_This.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_This.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_This.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Throw"></a>[module uglifyjs.AST_Throw](#apidoc.module.uglifyjs.AST_Throw)

#### <a name="apidoc.element.uglifyjs.AST_Throw.AST_Throw"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Throw (props)](#apidoc.element.uglifyjs.AST_Throw.AST_Throw)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Throw.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Throw.BASE)
- description and source-code
```javascript
function AST_Exit(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Throw.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Throw.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Throw.prototype"></a>[module uglifyjs.AST_Throw.prototype](#apidoc.module.uglifyjs.AST_Throw.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Throw.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Throw.prototype.CTOR)
- description and source-code
```javascript
function AST_Throw(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Throw.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Throw.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "throw");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Throw.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Throw.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Throw.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_Token"></a>[module uglifyjs.AST_Token](#apidoc.module.uglifyjs.AST_Token)

#### <a name="apidoc.element.uglifyjs.AST_Token.AST_Token"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Token (props)](#apidoc.element.uglifyjs.AST_Token.AST_Token)
- description and source-code
```javascript
function AST_Token(props){ if (props) { this.file = props.file;this.comments_before = props.comments_before;this.nlb = props.nlb
;this.endpos = props.endpos;this.endcol = props.endcol;this.endline = props.endline;this.pos = props.pos;this.col = props.col;this
.line = props.line;this.value = props.value;this.type = props.type;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Token.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Token.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Token.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Token.prototype"></a>[module uglifyjs.AST_Token.prototype](#apidoc.module.uglifyjs.AST_Token.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Token.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Token.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Token.prototype.CTOR)
- description and source-code
```javascript
function AST_Token(props){ if (props) { this.file = props.file;this.comments_before = props.comments_before;this.nlb = props.nlb
;this.endpos = props.endpos;this.endcol = props.endcol;this.endline = props.endline;this.pos = props.pos;this.col = props.col;this
.line = props.line;this.value = props.value;this.type = props.type;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```



# <a name="apidoc.module.uglifyjs.AST_Toplevel"></a>[module uglifyjs.AST_Toplevel](#apidoc.module.uglifyjs.AST_Toplevel)

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.AST_Toplevel"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Toplevel (props)](#apidoc.element.uglifyjs.AST_Toplevel.AST_Toplevel)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Toplevel.BASE)
- description and source-code
```javascript
function AST_Scope(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props.
cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Toplevel.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Toplevel.prototype"></a>[module uglifyjs.AST_Toplevel.prototype](#apidoc.module.uglifyjs.AST_Toplevel.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.CTOR)
- description and source-code
```javascript
function AST_Toplevel(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.cname = props
.cname;this.enclosed = props.enclosed;this.parent_scope = props.parent_scope;this.uses_eval = props.uses_eval;this.uses_with = props
.uses_with;this.functions = props.functions;this.variables = props.variables;this.directives = props.directives;this.globals = props
.globals;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Toplevel.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    display_body(self.body, true, output);
    output.print("");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype._default_mangler_options"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>_default_mangler_options (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype._default_mangler_options)
- description and source-code
```javascript
_default_mangler_options = function (options){
    return defaults(options, {
        except      : [],
        eval        : false,
        sort        : false,
        toplevel    : false,
        screw_ie8   : false,
        keep_fnames : false
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.compute_char_frequency"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>compute_char_frequency (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.compute_char_frequency)
- description and source-code
```javascript
compute_char_frequency = function (options){
    options = this._default_mangler_options(options);
    var tw = new TreeWalker(function(node){
        if (node instanceof AST_Constant)
            base54.consider(node.print_to_string());
        else if (node instanceof AST_Return)
            base54.consider("return");
        else if (node instanceof AST_Throw)
            base54.consider("throw");
        else if (node instanceof AST_Continue)
            base54.consider("continue");
        else if (node instanceof AST_Break)
            base54.consider("break");
        else if (node instanceof AST_Debugger)
            base54.consider("debugger");
        else if (node instanceof AST_Directive)
            base54.consider(node.value);
        else if (node instanceof AST_While)
            base54.consider("while");
        else if (node instanceof AST_Do)
            base54.consider("do while");
        else if (node instanceof AST_If) {
            base54.consider("if");
            if (node.alternative) base54.consider("else");
        }
        else if (node instanceof AST_Var)
            base54.consider("var");
        else if (node instanceof AST_Const)
            base54.consider("const");
        else if (node instanceof AST_Lambda)
            base54.consider("function");
        else if (node instanceof AST_For)
            base54.consider("for");
        else if (node instanceof AST_ForIn)
            base54.consider("for in");
        else if (node instanceof AST_Switch)
            base54.consider("switch");
        else if (node instanceof AST_Case)
            base54.consider("case");
        else if (node instanceof AST_Default)
            base54.consider("default");
        else if (node instanceof AST_With)
            base54.consider("with");
        else if (node instanceof AST_ObjectSetter)
            base54.consider("set" + node.key);
        else if (node instanceof AST_ObjectGetter)
            base54.consider("get" + node.key);
        else if (node instanceof AST_ObjectKeyVal)
            base54.consider(node.key);
        else if (node instanceof AST_New)
            base54.consider("new");
        else if (node instanceof AST_This)
            base54.consider("this");
        else if (node instanceof AST_Try)
            base54.consider("try");
        else if (node instanceof AST_Catch)
            base54.consider("catch");
        else if (node instanceof AST_Finally)
            base54.consider("finally");
        else if (node instanceof AST_Symbol && node.unmangleable(options))
            base54.consider(node.name);
        else if (node instanceof AST_Unary || node instanceof AST_Binary)
            base54.consider(node.operator);
        else if (node instanceof AST_Dot)
            base54.consider(node.property);
    });
    this.walk(tw);
    base54.sort();
}
```
- example usage
```shell
...
  // Compression
  uAST.figure_out_scope();
  uAST = uAST.transform(UglifyJS.Compressor(options));

  // Mangling (optional)
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''
...
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.figure_out_scope"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>figure_out_scope (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.figure_out_scope)
- description and source-code
```javascript
figure_out_scope = function (options){
    options = defaults(options, {
        screw_ie8: false
    });

    // pass 1: setup scope chaining and handle definitions
    var self = this;
    var scope = self.parent_scope = null;
    var defun = null;
    var nesting = 0;
    var tw = new TreeWalker(function(node, descend){
        if (options.screw_ie8 && node instanceof AST_Catch) {
            var save_scope = scope;
            scope = new AST_Scope(node);
            scope.init_scope_vars(nesting);
            scope.parent_scope = save_scope;
            descend();
            scope = save_scope;
            return true;
        }
        if (node instanceof AST_Scope) {
            node.init_scope_vars(nesting);
            var save_scope = node.parent_scope = scope;
            var save_defun = defun;
            defun = scope = node;
            ++nesting; descend(); --nesting;
            scope = save_scope;
            defun = save_defun;
            return true;        // don't descend again in TreeWalker
        }
        if (node instanceof AST_Directive) {
            node.scope = scope;
            push_uniq(scope.directives, node.value);
            return true;
        }
        if (node instanceof AST_With) {
            for (var s = scope; s; s = s.parent_scope)
                s.uses_with = true;
            return;
        }
        if (node instanceof AST_Symbol) {
            node.scope = scope;
        }
        if (node instanceof AST_SymbolLambda) {
            defun.def_function(node);
        }
        else if (node instanceof AST_SymbolDefun) {
            // Careful here, the scope where this should be defined is
            // the parent scope.  The reason is that we enter a new
            // scope when we encounter the AST_Defun node (which is
            // instanceof AST_Scope) but we get to the symbol a bit
            // later.
            (node.scope = defun.parent_scope).def_function(node);
        }
        else if (node instanceof AST_SymbolVar
                 || node instanceof AST_SymbolConst) {
            var def = defun.def_variable(node);
            def.constant = node instanceof AST_SymbolConst;
            def.init = tw.parent().value;
        }
        else if (node instanceof AST_SymbolCatch) {
            (options.screw_ie8 ? scope : defun)
                .def_variable(node);
        }
    });
    self.walk(tw);

    // pass 2: find back references and eval
    var func = null;
    var globals = self.globals = new Dictionary();
    var tw = new TreeWalker(function(node, descend){
        if (node instanceof AST_Lambda) {
            var prev_func = func;
            func = node;
            descend();
            func = prev_func;
            return true;
        }
        if (node instanceof AST_SymbolRef) {
            var name = node.name;
            var sym = node.scope.find_variable(name);
            if (!sym) {
                var g;
                if (globals.has(name)) {
                    g = globals.get(name);
                } else {
                    g = new SymbolDef(self, globals.size(), node);
                    g.undeclared = true;
                    g.global = true;
                    globals.set(name, g);
                }
                node.thedef = g;
                if (name == "eval" && tw.parent() instanceof AST_Call) {
                    for (var s = node.scope; s && !s.uses_eval; s = s.parent_scope)
                        s.uses_eval = true;
                }
                if (func && name == "arguments") {
                    func.uses_arguments = true;
                }
            } else {
                node.thedef = sym;
            }
            node.reference();
            return true;
        }
    });
    self.walk(tw);
}
```
- example usage
```shell
...

'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
...
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.mangle_names"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>mangle_names (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.mangle_names)
- description and source-code
```javascript
mangle_names = function (options){
    options = this._default_mangler_options(options);
    // We only need to mangle declaration nodes.  Special logic wired
    // into the code generator will display the mangled name if it's
    // present (and for AST_SymbolRef-s it'll use the mangled name of
    // the AST_SymbolDeclaration that it points to).
    var lname = -1;
    var to_mangle = [];
    var tw = new TreeWalker(function(node, descend){
        if (node instanceof AST_LabeledStatement) {
            // lname is incremented when we get to the AST_Label
            var save_nesting = lname;
            descend();
            lname = save_nesting;
            return true;        // don't descend again in TreeWalker
        }
        if (node instanceof AST_Scope) {
            var p = tw.parent(), a = [];
            node.variables.each(function(symbol){
                if (options.except.indexOf(symbol.name) < 0) {
                    a.push(symbol);
                }
            });
            if (options.sort) a.sort(function(a, b){
                return b.references.length - a.references.length;
            });
            to_mangle.push.apply(to_mangle, a);
            return;
        }
        if (node instanceof AST_Label) {
            var name;
            do name = base54(++lname); while (!is_identifier(name));
            node.mangled_name = name;
            return true;
        }
        if (options.screw_ie8 && node instanceof AST_SymbolCatch) {
            to_mangle.push(node.definition());
            return;
        }
    });
    this.walk(tw);
    to_mangle.forEach(function(def){ def.mangle(options) });
}
```
- example usage
```shell
...
  uAST.figure_out_scope();
  uAST = uAST.transform(UglifyJS.Compressor(options));

  // Mangling (optional)
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''
...
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.scope_warnings"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>scope_warnings (options)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.scope_warnings)
- description and source-code
```javascript
scope_warnings = function (options){
    options = defaults(options, {
        undeclared       : false, // this makes a lot of noise
        unreferenced     : true,
        assign_to_global : true,
        func_arguments   : true,
        nested_defuns    : true,
        eval             : true
    });
    var tw = new TreeWalker(function(node){
        if (options.undeclared
            && node instanceof AST_SymbolRef
            && node.undeclared())
        {
            // XXX: this also warns about JS standard names,
            // i.e. Object, Array, parseInt etc.  Should add a list of
            // exceptions.
            AST_Node.warn("Undeclared symbol: {name} [{file}:{line},{col}]", {
                name: node.name,
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
        if (options.assign_to_global)
        {
            var sym = null;
            if (node instanceof AST_Assign && node.left instanceof AST_SymbolRef)
                sym = node.left;
            else if (node instanceof AST_ForIn && node.init instanceof AST_SymbolRef)
                sym = node.init;
            if (sym
                && (sym.undeclared()
                    || (sym.global() && sym.scope !== sym.definition().scope))) {
                AST_Node.warn("{msg}: {name} [{file}:{line},{col}]", {
                    msg: sym.undeclared() ? "Accidental global?" : "Assignment to global",
                    name: sym.name,
                    file: sym.start.file,
                    line: sym.start.line,
                    col: sym.start.col
                });
            }
        }
        if (options.eval
            && node instanceof AST_SymbolRef
            && node.undeclared()
            && node.name == "eval") {
            AST_Node.warn("Eval is used [{file}:{line},{col}]", node.start);
        }
        if (options.unreferenced
            && (node instanceof AST_SymbolDeclaration || node instanceof AST_Label)
            && !(node instanceof AST_SymbolCatch)
            && node.unreferenced()) {
            AST_Node.warn("{type} {name} is declared but not referenced [{file}:{line},{col}]", {
                type: node instanceof AST_Label ? "Label" : "Symbol",
                name: node.name,
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
        if (options.func_arguments
            && node instanceof AST_Lambda
            && node.uses_arguments) {
            AST_Node.warn("arguments used in function {name} [{file}:{line},{col}]", {
                name: node.name ? node.name.name : "anonymous",
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
        if (options.nested_defuns
            && node instanceof AST_Defun
            && !(tw.parent() instanceof AST_Scope)) {
            AST_Node.warn("Function {name} declared in nested statement \"{type}\" [{file}:{line},{col}]", {
                name: node.name.name,
                type: tw.parent().TYPE,
                file: node.start.file,
                line: node.start.line,
                col: node.start.col
            });
        }
    });
    this.walk(tw);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Toplevel.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.wrap_commonjs"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>wrap_commonjs (name, export_all)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.wrap_commonjs)
- description and source-code
```javascript
wrap_commonjs = function (name, export_all) {
    var self = this;
    var to_export = [];
    if (export_all) {
        self.figure_out_scope();
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_SymbolDeclaration && node.definition().global) {
                if (!find_if(function(n){ return n.name == node.name }, to_export))
                    to_export.push(node);
            }
        }));
    }
    var wrapped_tl = "(function(exports, global){ global['" + name + "'] = exports; '$ORIG'; '$EXPORTS'; }({}, (function(){return
 this}())))";
    wrapped_tl = parse(wrapped_tl);
    wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
        if (node instanceof AST_SimpleStatement) {
            node = node.body;
            if (node instanceof AST_String) switch (node.getValue()) {
              case "$ORIG":
                return MAP.splice(self.body);
              case "$EXPORTS":
                var body = [];
                to_export.forEach(function(sym){
                    body.push(new AST_SimpleStatement({
                        body: new AST_Assign({
                            left: new AST_Sub({
                                expression: new AST_SymbolRef({ name: "exports" }),
                                property: new AST_String({ value: sym.name }),
                            }),
                            operator: "=",
                            right: new AST_SymbolRef(sym),
                        }),
                    }));
                });
                return MAP.splice(body);
            }
        }
    }));
    return wrapped_tl;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Toplevel.prototype.wrap_enclose"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Toplevel.prototype.</span>wrap_enclose (arg_parameter_pairs)](#apidoc.element.uglifyjs.AST_Toplevel.prototype.wrap_enclose)
- description and source-code
```javascript
wrap_enclose = function (arg_parameter_pairs) {
    var self = this;
    var args = [];
    var parameters = [];

    arg_parameter_pairs.forEach(function(pair) {
        var splitAt = pair.lastIndexOf(":");

        args.push(pair.substr(0, splitAt));
        parameters.push(pair.substr(splitAt + 1));
    });

    var wrapped_tl = "(function(" + parameters.join(",") + "){ '$ORIG'; })(" + args.join(",") + ")";
    wrapped_tl = parse(wrapped_tl);
    wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
        if (node instanceof AST_Directive && node.value == "$ORIG") {
            return MAP.splice(self.body);
        }
    }));
    return wrapped_tl;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_True"></a>[module uglifyjs.AST_True](#apidoc.module.uglifyjs.AST_True)

#### <a name="apidoc.element.uglifyjs.AST_True.AST_True"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_True (props)](#apidoc.element.uglifyjs.AST_True.AST_True)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_True.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>BASE (props)](#apidoc.element.uglifyjs.AST_True.BASE)
- description and source-code
```javascript
function AST_Boolean(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_True.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_True.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_True.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_True.prototype"></a>[module uglifyjs.AST_True.prototype](#apidoc.module.uglifyjs.AST_True.prototype)

#### <a name="apidoc.element.uglifyjs.AST_True.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_True.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_True.prototype.CTOR)
- description and source-code
```javascript
function AST_True(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_True.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_True.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_True.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){ return true }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Try"></a>[module uglifyjs.AST_Try](#apidoc.module.uglifyjs.AST_Try)

#### <a name="apidoc.element.uglifyjs.AST_Try.AST_Try"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Try (props)](#apidoc.element.uglifyjs.AST_Try.AST_Try)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Try.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Try.BASE)
- description and source-code
```javascript
function AST_Block(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Try.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Try.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Try.prototype"></a>[module uglifyjs.AST_Try.prototype](#apidoc.module.uglifyjs.AST_Try.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Try.prototype.CTOR)
- description and source-code
```javascript
function AST_Try(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.bfinally = props
.bfinally;this.bcatch = props.bcatch;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Try.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("try");
    output.space();
    print_bracketed(self.body, output);
    if (self.bcatch) {
        output.space();
        self.bcatch.print(output);
    }
    if (self.bfinally) {
        output.space();
        self.bfinally.print(output);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Try.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        walk_body(this, visitor);
        if (this.bcatch) this.bcatch._walk(visitor);
        if (this.bfinally) this.bfinally._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype.add_source_map"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>add_source_map (stream)](#apidoc.element.uglifyjs.AST_Try.prototype.add_source_map)
- description and source-code
```javascript
add_source_map = function (stream){
    generator(this, stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Try.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Try.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Try.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Try.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Try.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_Unary"></a>[module uglifyjs.AST_Unary](#apidoc.module.uglifyjs.AST_Unary)

#### <a name="apidoc.element.uglifyjs.AST_Unary.AST_Unary"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Unary (props)](#apidoc.element.uglifyjs.AST_Unary.AST_Unary)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Unary.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Unary.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Unary.SUBCLASSES"></a>[module uglifyjs.AST_Unary.SUBCLASSES](#apidoc.module.uglifyjs.AST_Unary.SUBCLASSES)

#### <a name="apidoc.element.uglifyjs.AST_Unary.SUBCLASSES.0"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.SUBCLASSES.</span>0 (props)](#apidoc.element.uglifyjs.AST_Unary.SUBCLASSES.0)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.SUBCLASSES.1"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.SUBCLASSES.</span>1 (props)](#apidoc.element.uglifyjs.AST_Unary.SUBCLASSES.1)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Unary.prototype"></a>[module uglifyjs.AST_Unary.prototype](#apidoc.module.uglifyjs.AST_Unary.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Unary.prototype.CTOR)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_Unary.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype.has_side_effects"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>has_side_effects (compressor)](#apidoc.element.uglifyjs.AST_Unary.prototype.has_side_effects)
- description and source-code
```javascript
has_side_effects = function (compressor){
    return this.operator == "delete"
        || this.operator == "++"
        || this.operator == "--"
        || this.expression.has_side_effects(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype.lift_sequences"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>lift_sequences (compressor)](#apidoc.element.uglifyjs.AST_Unary.prototype.lift_sequences)
- description and source-code
```javascript
lift_sequences = function (compressor){
    if (compressor.option("sequences")) {
        if (this.expression instanceof AST_Seq) {
            var seq = this.expression;
            var x = seq.to_array();
            this.expression = x.pop();
            x.push(this);
            seq = AST_Seq.from_array(x).transform(compressor);
            return seq;
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Unary.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    return p instanceof AST_PropAccess && p.expression === this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_Unary.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_Unary.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Unary.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_Unary.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_UnaryPostfix"></a>[module uglifyjs.AST_UnaryPostfix](#apidoc.module.uglifyjs.AST_UnaryPostfix)

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix.AST_UnaryPostfix"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPostfix (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix.AST_UnaryPostfix)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>BASE (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix.BASE)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_UnaryPostfix.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_UnaryPostfix.prototype"></a>[module uglifyjs.AST_UnaryPostfix.prototype](#apidoc.module.uglifyjs.AST_UnaryPostfix.prototype)

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_UnaryPostfix.prototype.CTOR)
- description and source-code
```javascript
function AST_UnaryPostfix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;
this.operator = props.operator;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_UnaryPostfix.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.expression.print(output);
    output.print(self.operator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPostfix.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPostfix.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_UnaryPostfix.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_UnaryPrefix"></a>[module uglifyjs.AST_UnaryPrefix](#apidoc.module.uglifyjs.AST_UnaryPrefix)

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.AST_UnaryPrefix"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_UnaryPrefix (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix.AST_UnaryPrefix)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>BASE (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix.BASE)
- description and source-code
```javascript
function AST_Unary(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this.operator
 = props.operator;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_UnaryPrefix.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_UnaryPrefix.prototype"></a>[module uglifyjs.AST_UnaryPrefix.prototype](#apidoc.module.uglifyjs.AST_UnaryPrefix.prototype)

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.CTOR)
- description and source-code
```javascript
function AST_UnaryPrefix(props){ if (props) { this.end = props.end;this.start = props.start;this.expression = props.expression;this
.operator = props.operator;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    var op = self.operator;
    output.print(op);
    if (/^[a-z]/i.test(op)
        || (/[+-]$/.test(op)
            && self.expression instanceof AST_UnaryPrefix
            && /^[+-]/.test(self.expression.operator))) {
        output.space();
    }
    self.expression.print(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype._eval"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>_eval (compressor)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype._eval)
- description and source-code
```javascript
_eval = function (compressor){
    var e = this.expression;
    switch (this.operator) {
      case "!": return !ev(e, compressor);
      case "typeof":
        // Function would be evaluated to an array and so typeof would
        // incorrectly return 'object'. Hence making is a special case.
        if (e instanceof AST_Function) return typeof function(){};

        e = ev(e, compressor);

        // typeof <RegExp> returns "object" or "function" on different platforms
        // so cannot evaluate reliably
        if (e instanceof RegExp) throw def;

        return typeof e;
      case "void": return void ev(e, compressor);
      case "~": return ~ev(e, compressor);
      case "-":
        e = ev(e, compressor);
        if (e === 0) throw def;
        return -e;
      case "+": return +ev(e, compressor);
    }
    throw def;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.is_boolean"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>is_boolean ()](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.is_boolean)
- description and source-code
```javascript
is_boolean = function (){
    return member(this.operator, unary_bool);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.is_string"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>is_string ()](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.is_string)
- description and source-code
```javascript
is_string = function (){
    return this.operator == "typeof";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.negate"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>negate (compressor)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.negate)
- description and source-code
```javascript
negate = function (compressor){
    return func.call(this, compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_UnaryPrefix.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_UnaryPrefix.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Undefined"></a>[module uglifyjs.AST_Undefined](#apidoc.module.uglifyjs.AST_Undefined)

#### <a name="apidoc.element.uglifyjs.AST_Undefined.AST_Undefined"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Undefined (props)](#apidoc.element.uglifyjs.AST_Undefined.AST_Undefined)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Undefined.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Undefined.BASE)
- description and source-code
```javascript
function AST_Atom(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Undefined.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Undefined.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Undefined.prototype"></a>[module uglifyjs.AST_Undefined.prototype](#apidoc.module.uglifyjs.AST_Undefined.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Undefined.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Undefined.prototype.CTOR)
- description and source-code
```javascript
function AST_Undefined(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Undefined.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Undefined.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("void 0");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Undefined.prototype.needs_parens"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>needs_parens (output)](#apidoc.element.uglifyjs.AST_Undefined.prototype.needs_parens)
- description and source-code
```javascript
needs_parens = function (output){
    var p = output.parent();
    return p instanceof AST_PropAccess && p.expression === this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Undefined.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Undefined.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_Undefined.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Var"></a>[module uglifyjs.AST_Var](#apidoc.module.uglifyjs.AST_Var)

#### <a name="apidoc.element.uglifyjs.AST_Var.AST_Var"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_Var (props)](#apidoc.element.uglifyjs.AST_Var.AST_Var)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Var.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>BASE (props)](#apidoc.element.uglifyjs.AST_Var.BASE)
- description and source-code
```javascript
function AST_Definitions(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions
;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_Var.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Var.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_Var.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_Var.prototype"></a>[module uglifyjs.AST_Var.prototype](#apidoc.module.uglifyjs.AST_Var.prototype)

#### <a name="apidoc.element.uglifyjs.AST_Var.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Var.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_Var.prototype.CTOR)
- description and source-code
```javascript
function AST_Var(props){ if (props) { this.end = props.end;this.start = props.start;this.definitions = props.definitions;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_Var.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_Var.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_Var.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self._do_print(output, "var");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_VarDef"></a>[module uglifyjs.AST_VarDef](#apidoc.module.uglifyjs.AST_VarDef)

#### <a name="apidoc.element.uglifyjs.AST_VarDef.AST_VarDef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_VarDef (props)](#apidoc.element.uglifyjs.AST_VarDef.AST_VarDef)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>BASE (props)](#apidoc.element.uglifyjs.AST_VarDef.BASE)
- description and source-code
```javascript
function AST_Node(props){ if (props) { this.end = props.end;this.start = props.start;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_VarDef.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_VarDef.prototype"></a>[module uglifyjs.AST_VarDef.prototype](#apidoc.module.uglifyjs.AST_VarDef.prototype)

#### <a name="apidoc.element.uglifyjs.AST_VarDef.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_VarDef.prototype.CTOR)
- description and source-code
```javascript
function AST_VarDef(props){ if (props) { this.end = props.end;this.start = props.start;this.value = props.value;this.name = props
.name;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_VarDef.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    self.name.print(output);
    if (self.value) {
        output.space();
        output.print("=");
        output.space();
        var p = output.parent(1);
        var noin = p instanceof AST_For || p instanceof AST_ForIn;
        parenthesize_for_noin(self.value, output, noin);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_VarDef.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.name._walk(visitor);
        if (this.value) this.value._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_VarDef.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_VarDef.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_VarDef.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_VarDef.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.AST_While"></a>[module uglifyjs.AST_While](#apidoc.module.uglifyjs.AST_While)

#### <a name="apidoc.element.uglifyjs.AST_While.AST_While"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_While (props)](#apidoc.element.uglifyjs.AST_While.AST_While)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_While.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>BASE (props)](#apidoc.element.uglifyjs.AST_While.BASE)
- description and source-code
```javascript
function AST_DWLoop(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_While.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_While.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_While.prototype"></a>[module uglifyjs.AST_While.prototype](#apidoc.module.uglifyjs.AST_While.prototype)

#### <a name="apidoc.element.uglifyjs.AST_While.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_While.prototype.CTOR)
- description and source-code
```javascript
function AST_While(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.condition = props
.condition;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_While.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_While.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("while");
    output.space();
    output.with_parens(function(){
        self.condition.print(output);
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_While.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_While.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.condition._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_While.prototype.optimize"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>optimize (compressor)](#apidoc.element.uglifyjs.AST_While.prototype.optimize)
- description and source-code
```javascript
optimize = function (compressor){
    var self = this;
    if (self._optimized) return self;
    var opt = optimizer(self, compressor);
    opt._optimized = true;
    if (opt === self) return opt;
    return opt.transform(compressor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_While.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_While.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_While.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```



# <a name="apidoc.module.uglifyjs.AST_With"></a>[module uglifyjs.AST_With](#apidoc.module.uglifyjs.AST_With)

#### <a name="apidoc.element.uglifyjs.AST_With.AST_With"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>AST_With (props)](#apidoc.element.uglifyjs.AST_With.AST_With)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_With.BASE"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>BASE (props)](#apidoc.element.uglifyjs.AST_With.BASE)
- description and source-code
```javascript
function AST_StatementWithBody(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_With.DEFMETHOD"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.</span>DEFMETHOD (name, method)](#apidoc.element.uglifyjs.AST_With.DEFMETHOD)
- description and source-code
```javascript
DEFMETHOD = function (name, method) {
    this.prototype[name] = method;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.AST_With.prototype"></a>[module uglifyjs.AST_With.prototype](#apidoc.module.uglifyjs.AST_With.prototype)

#### <a name="apidoc.element.uglifyjs.AST_With.prototype.CTOR"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>CTOR (props)](#apidoc.element.uglifyjs.AST_With.prototype.CTOR)
- description and source-code
```javascript
function AST_With(props){ if (props) { this.end = props.end;this.start = props.start;this.body = props.body;this.expression = props
.expression;}}
```
- example usage
```shell
...
};

var AST_Token = DEFNODE("Token", "type value line col pos endline endcol endpos nlb comments_before file", {
}, null);

var AST_Node = DEFNODE("Node", "start end", {
clone: function() {
    return new this.CTOR(this);
},
$documentation: "Base class of all AST nodes",
$propdoc: {
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
...
```

#### <a name="apidoc.element.uglifyjs.AST_With.prototype._codegen"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>_codegen (self, output)](#apidoc.element.uglifyjs.AST_With.prototype._codegen)
- description and source-code
```javascript
_codegen = function (self, output){
    output.print("with");
    output.space();
    output.with_parens(function(){
        self.expression.print(output);
    });
    output.space();
    self._do_print_body(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.AST_With.prototype._walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>_walk (visitor)](#apidoc.element.uglifyjs.AST_With.prototype._walk)
- description and source-code
```javascript
_walk = function (visitor) {
    return visitor._visit(this, function(){
        this.expression._walk(visitor);
        this.body._walk(visitor);
    });
}
```
- example usage
```shell
...
    start: "[AST_Token] The first token of this node",
    end: "[AST_Token] The last token of this node"
},
_walk: function(visitor) {
    return visitor._visit(this);
},
walk: function(visitor) {
    return this._walk(visitor); // not sure the indirection will be any help
}
}, null);

AST_Node.warn_function = null;
AST_Node.warn = function(txt, props) {
if (AST_Node.warn_function)
    AST_Node.warn_function(string_template(txt, props));
...
```

#### <a name="apidoc.element.uglifyjs.AST_With.prototype.to_mozilla_ast"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>to_mozilla_ast ()](#apidoc.element.uglifyjs.AST_With.prototype.to_mozilla_ast)
- description and source-code
```javascript
to_mozilla_ast = function () {
    return set_moz_loc(this, handler(this));
}
```
- example usage
```shell
...
  if (mangle) {
    uAST.figure_out_scope();
    uAST.compute_char_frequency();
    uAST.mangle_names();
  }

  // Back-conversion to SpiderMonkey AST
  return uAST.to_mozilla_ast();
}
'''

Check out
[original blog post](http://rreverser.com/using-mozilla-ast-with-uglifyjs/)
for details.
...
```

#### <a name="apidoc.element.uglifyjs.AST_With.prototype.transform"></a>[function <span class="apidocSignatureSpan">uglifyjs.AST_With.prototype.</span>transform (tw, in_list)](#apidoc.element.uglifyjs.AST_With.prototype.transform)
- description and source-code
```javascript
transform = function (tw, in_list){
    var x, y;
    tw.push(this);
    if (tw.before) x = tw.before(this, descend, in_list);
    if (x === undefined) {
        if (!tw.after) {
            x = this;
            descend(x, tw);
        } else {
            tw.stack[tw.stack.length - 1] = x = this.clone();
            descend(x, tw);
            y = tw.after(x, in_list);
            if (y !== undefined) x = y;
        }
    }
    tw.pop();
    return x;
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.Buffer"></a>[module uglifyjs.Buffer](#apidoc.module.uglifyjs.Buffer)

#### <a name="apidoc.element.uglifyjs.Buffer.Buffer"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.uglifyjs.Buffer.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.alloc"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>alloc (size, fill, encoding)](#apidoc.element.uglifyjs.Buffer.alloc)
- description and source-code
```javascript
alloc = function (size, fill, encoding) {
  assertSize(size);
  if (size > 0 && fill !== undefined) {
    // Since we are filling anyway, don't zero fill initially.
    // Only pay attention to encoding if it's a string. This
    // prevents accidentally sending in a number that would
    // be interpretted as a start offset.
    if (typeof encoding !== 'string')
      encoding = undefined;
    return createUnsafeBuffer(size).fill(fill, encoding);
  }
  return new FastBuffer(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.allocUnsafe"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>allocUnsafe (size)](#apidoc.element.uglifyjs.Buffer.allocUnsafe)
- description and source-code
```javascript
allocUnsafe = function (size) {
  assertSize(size);
  return allocate(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.allocUnsafeSlow"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>allocUnsafeSlow (size)](#apidoc.element.uglifyjs.Buffer.allocUnsafeSlow)
- description and source-code
```javascript
allocUnsafeSlow = function (size) {
  assertSize(size);
  return createUnsafeBuffer(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.byteLength"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>byteLength (string, encoding)](#apidoc.element.uglifyjs.Buffer.byteLength)
- description and source-code
```javascript
function byteLength(string, encoding) {
  if (typeof string !== 'string') {
    if (ArrayBuffer.isView(string) || isArrayBuffer(string) ||
        isSharedArrayBuffer(string)) {
      return string.byteLength;
    }

    string = '' + string;
  }

  var len = string.length;
  if (len === 0)
    return 0;

  // Use a for loop to avoid recursion
  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'ascii':
      case 'latin1':
      case 'binary':
        return len;

      case 'utf8':
      case 'utf-8':
      case undefined:
        return binding.byteLengthUtf8(string);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return len * 2;

      case 'hex':
        return len >>> 1;

      case 'base64':
        return base64ByteLength(string, len);

      default:
        // The C++ binding defaulted to UTF8, we should too.
        if (loweredCase)
          return binding.byteLengthUtf8(string);

        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.compare"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>compare (a, b)](#apidoc.element.uglifyjs.Buffer.compare)
- description and source-code
```javascript
function compare(a, b) {
  if (!(a instanceof Buffer) ||
      !(b instanceof Buffer)) {
    throw new TypeError('Arguments must be Buffers');
  }

  if (a === b) {
    return 0;
  }

  return binding.compare(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.concat"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>concat (list, length)](#apidoc.element.uglifyjs.Buffer.concat)
- description and source-code
```javascript
concat = function (list, length) {
  var i;
  if (!Array.isArray(list))
    throw new TypeError('"list" argument must be an Array of Buffers');

  if (list.length === 0)
    return new FastBuffer();

  if (length === undefined) {
    length = 0;
    for (i = 0; i < list.length; i++)
      length += list[i].length;
  } else {
    length = length >>> 0;
  }

  var buffer = Buffer.allocUnsafe(length);
  var pos = 0;
  for (i = 0; i < list.length; i++) {
    var buf = list[i];
    if (!Buffer.isBuffer(buf))
      throw new TypeError('"list" argument must be an Array of Buffers');
    buf.copy(buffer, pos);
    pos += buf.length;
  }

  // Note: 'length' is always equal to 'buffer.length' at this point
  if (pos < length) {
    // Zero-fill the remaining bytes if the specified 'length' was more than
    // the actual total length, i.e. if we have some remaining allocated bytes
    // there were not initialized.
    buffer.fill(0, pos, length);
  }

  return buffer;
}
```
- example usage
```shell
...

function DEFNODE(type, props, methods, base) {
if (arguments.length < 4) base = AST_Node;
if (!props) props = [];
else props = props.split(/\s+/);
var self_props = props;
if (base && base.PROPS)
    props = props.concat(base.PROPS);
var code = "return function AST_" + type + "(props){ if (props) { ";
for (var i = props.length; --i >= 0;) {
    code += "this." + props[i] + " = props." + props[i] + ";";
}
var proto = base && new base;
if (proto && proto.initialize || (methods && methods.initialize))
    code += "this.initialize();";
...
```

#### <a name="apidoc.element.uglifyjs.Buffer.from"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>from (value, encodingOrOffset, length)](#apidoc.element.uglifyjs.Buffer.from)
- description and source-code
```javascript
from = function (value, encodingOrOffset, length) {
  if (typeof value === 'number')
    throw new TypeError('"value" argument must not be a number');

  if (isArrayBuffer(value) || isSharedArrayBuffer(value))
    return fromArrayBuffer(value, encodingOrOffset, length);

  if (typeof value === 'string')
    return fromString(value, encodingOrOffset);

  return fromObject(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.isBuffer"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>isBuffer (b)](#apidoc.element.uglifyjs.Buffer.isBuffer)
- description and source-code
```javascript
function isBuffer(b) {
  return b instanceof Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.isEncoding"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.</span>isEncoding (encoding)](#apidoc.element.uglifyjs.Buffer.isEncoding)
- description and source-code
```javascript
isEncoding = function (encoding) {
  return typeof encoding === 'string' &&
         typeof internalUtil.normalizeEncoding(encoding) === 'string';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.Buffer.prototype"></a>[module uglifyjs.Buffer.prototype](#apidoc.module.uglifyjs.Buffer.prototype)

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.asciiSlice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.uglifyjs.Buffer.prototype.asciiSlice)
- description and source-code
```javascript
function asciiSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.asciiWrite"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.uglifyjs.Buffer.prototype.asciiWrite)
- description and source-code
```javascript
function asciiWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.base64Slice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>base64Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.base64Slice)
- description and source-code
```javascript
function base64Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.base64Write"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>base64Write ()](#apidoc.element.uglifyjs.Buffer.prototype.base64Write)
- description and source-code
```javascript
function base64Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.compare"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.uglifyjs.Buffer.prototype.compare)
- description and source-code
```javascript
function compare(target, start, end, thisStart, thisEnd) {

  if (!(target instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');
  if (arguments.length === 1)
    return compare_(this, target);

  if (start === undefined)
    start = 0;
  else if (start < 0)
    throw new RangeError('out of range index');
  else
    start >>>= 0;

  if (end === undefined)
    end = target.length;
  else if (end > target.length)
    throw new RangeError('out of range index');
  else
    end >>>= 0;

  if (thisStart === undefined)
    thisStart = 0;
  else if (thisStart < 0)
    throw new RangeError('out of range index');
  else
    thisStart >>>= 0;

  if (thisEnd === undefined)
    thisEnd = this.length;
  else if (thisEnd > this.length)
    throw new RangeError('out of range index');
  else
    thisEnd >>>= 0;

  if (thisStart >= thisEnd)
    return (start >= end ? 0 : -1);
  else if (start >= end)
    return 1;

  return compareOffset(this, target, start, thisStart, end, thisEnd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.copy"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>copy ()](#apidoc.element.uglifyjs.Buffer.prototype.copy)
- description and source-code
```javascript
function copy() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.equals"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>equals (b)](#apidoc.element.uglifyjs.Buffer.prototype.equals)
- description and source-code
```javascript
function equals(b) {
  if (!(b instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');

  if (this === b)
    return true;

  return binding.compare(this, b) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.fill"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.fill)
- description and source-code
```javascript
function fill(val, start, end, encoding) {
  // Handle string cases:
  if (typeof val === 'string') {
    if (typeof start === 'string') {
      encoding = start;
      start = 0;
      end = this.length;
    } else if (typeof end === 'string') {
      encoding = end;
      end = this.length;
    }

    if (encoding !== undefined && typeof encoding !== 'string') {
      throw new TypeError('encoding must be a string');
    }
    var normalizedEncoding = internalUtil.normalizeEncoding(encoding);
    if (normalizedEncoding === undefined) {
      throw new TypeError('Unknown encoding: ' + encoding);
    }

    if (val.length === 0) {
      // Previously, if val === '', the Buffer would not fill,
      // which is rather surprising.
      val = 0;
    } else if (val.length === 1) {
      var code = val.charCodeAt(0);
      if ((normalizedEncoding === 'utf8' && code < 128) ||
          normalizedEncoding === 'latin1') {
        // Fast path: If 'val' fits into a single byte, use that numeric value.
        val = code;
      }
    }
  } else if (typeof val === 'number') {
    val = val & 255;
  }

  // Invalid ranges are not set to a default, so can range check early.
  if (start < 0 || end > this.length)
    throw new RangeError('Out of range index');

  if (end <= start)
    return this;

  start = start >>> 0;
  end = end === undefined ? this.length : end >>> 0;

  binding.fill(this, val, start, end, encoding);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.hexSlice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>hexSlice ()](#apidoc.element.uglifyjs.Buffer.prototype.hexSlice)
- description and source-code
```javascript
function hexSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.hexWrite"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>hexWrite ()](#apidoc.element.uglifyjs.Buffer.prototype.hexWrite)
- description and source-code
```javascript
function hexWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.includes"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.includes)
- description and source-code
```javascript
function includes(val, byteOffset, encoding) {
  return this.indexOf(val, byteOffset, encoding) !== -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.indexOf)
- description and source-code
```javascript
function indexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, true);
}
```
- example usage
```shell
...
function AtTop(val) { this.v = val };
function Splice(val) { this.v = val };
function Last(val) { this.v = val };
return MAP;
})();

function push_uniq(array, el) {
if (array.indexOf(el) < 0)
    array.push(el);
};

function string_template(text, props) {
return text.replace(/\{(.+?)\}/g, function(str, p){
    return props[p];
});
...
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.inspect"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>inspect ()](#apidoc.element.uglifyjs.Buffer.prototype.inspect)
- description and source-code
```javascript
function inspect() {
  var str = '';
  var max = exports.INSPECT_MAX_BYTES;
  if (this.length > 0) {
    str = this.toString('hex', 0, max).match(/.{2}/g).join(' ');
    if (this.length > max)
      str += ' ... ';
  }
  return '<' + this.constructor.name + ' ' + str + '>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, false);
}
```
- example usage
```shell
...
    },
    wrap_enclose: function(arg_parameter_pairs) {
var self = this;
var args = [];
var parameters = [];

arg_parameter_pairs.forEach(function(pair) {
    var splitAt = pair.lastIndexOf(":");

    args.push(pair.substr(0, splitAt));
    parameters.push(pair.substr(splitAt + 1));
});

var wrapped_tl = "(function(" + parameters.join(",") + "){ '$ORIG'; })(" + args.join(",") + ")";
wrapped_tl = parse(wrapped_tl);
...
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.latin1Slice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.latin1Slice)
- description and source-code
```javascript
function latin1Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.latin1Write"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>latin1Write ()](#apidoc.element.uglifyjs.Buffer.prototype.latin1Write)
- description and source-code
```javascript
function latin1Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readDoubleBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readDoubleBE)
- description and source-code
```javascript
function readDoubleBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readDoubleLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readDoubleLE)
- description and source-code
```javascript
function readDoubleLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readFloatBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readFloatBE)
- description and source-code
```javascript
function readFloatBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readFloatLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readFloatLE)
- description and source-code
```javascript
function readFloatLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readInt16BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt16BE)
- description and source-code
```javascript
readInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset + 1] | (this[offset] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readInt16LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt16LE)
- description and source-code
```javascript
readInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset] | (this[offset + 1] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readInt32BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt32BE)
- description and source-code
```javascript
readInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] << 24) |
      (this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      (this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readInt32LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt32LE)
- description and source-code
```javascript
readInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16) |
      (this[offset + 3] << 24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readInt8"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readInt8)
- description and source-code
```javascript
readInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  var val = this[offset];
  return !(val & 0x80) ? val : (0xff - val + 1) * -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readIntBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readIntBE)
- description and source-code
```javascript
readIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var i = byteLength;
  var mul = 1;
  var val = this[offset + --i];
  while (i > 0 && (mul *= 0x100))
    val += this[offset + --i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readIntLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readIntLE)
- description and source-code
```javascript
readIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUInt16BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt16BE)
- description and source-code
```javascript
readUInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return (this[offset] << 8) | this[offset + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUInt16LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt16LE)
- description and source-code
```javascript
readUInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return this[offset] | (this[offset + 1] << 8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUInt32BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt32BE)
- description and source-code
```javascript
readUInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] * 0x1000000) +
      ((this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUInt32LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt32LE)
- description and source-code
```javascript
readUInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return ((this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16)) +
      (this[offset + 3] * 0x1000000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUInt8"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUInt8)
- description and source-code
```javascript
readUInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  return this[offset];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUIntBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUIntBE)
- description and source-code
```javascript
readUIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset + --byteLength];
  var mul = 1;
  while (byteLength > 0 && (mul *= 0x100))
    val += this[offset + --byteLength] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.readUIntLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.readUIntLE)
- description and source-code
```javascript
readUIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.slice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>slice (start, end)](#apidoc.element.uglifyjs.Buffer.prototype.slice)
- description and source-code
```javascript
function slice(start, end) {
  const srcLength = this.length;
  start = adjustOffset(start, srcLength);
  end = end !== undefined ? adjustOffset(end, srcLength) : srcLength;
  const newLength = end > start ? end - start : 0;
  return new FastBuffer(this.buffer, this.byteOffset + start, newLength);
}
```
- example usage
```shell
...
        function doit() {
var val = f(a[i], i);
var is_last = val instanceof Last;
if (is_last) val = val.v;
if (val instanceof AtTop) {
    val = val.v;
    if (val instanceof Splice) {
        top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
    } else {
        top.push(val);
    }
}
else if (val !== skip) {
    if (val instanceof Splice) {
        ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
...
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.swap16"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>swap16 ()](#apidoc.element.uglifyjs.Buffer.prototype.swap16)
- description and source-code
```javascript
function swap16() {
  // For Buffer.length < 128, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 2 !== 0)
    throw new RangeError('Buffer size must be a multiple of 16-bits');
  if (len < 128) {
    for (var i = 0; i < len; i += 2)
      swap(this, i, i + 1);
    return this;
  }
  return swap16n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.swap32"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>swap32 ()](#apidoc.element.uglifyjs.Buffer.prototype.swap32)
- description and source-code
```javascript
function swap32() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 4 !== 0)
    throw new RangeError('Buffer size must be a multiple of 32-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 4) {
      swap(this, i, i + 3);
      swap(this, i + 1, i + 2);
    }
    return this;
  }
  return swap32n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.swap64"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>swap64 ()](#apidoc.element.uglifyjs.Buffer.prototype.swap64)
- description and source-code
```javascript
function swap64() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 8 !== 0)
    throw new RangeError('Buffer size must be a multiple of 64-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 8) {
      swap(this, i, i + 7);
      swap(this, i + 1, i + 6);
      swap(this, i + 2, i + 5);
      swap(this, i + 3, i + 4);
    }
    return this;
  }
  return swap64n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>toJSON ()](#apidoc.element.uglifyjs.Buffer.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this.length) {
    const data = [];
    for (var i = 0; i < this.length; ++i)
      data[i] = this[i];
    return { type: 'Buffer', data };
  } else {
    return { type: 'Buffer', data: [] };
  }
}
```
- example usage
```shell
...
            source    : source,
            name      : name
        });
    }
    return {
        add        : add,
        get        : function() { return generator },
        toString   : function() { return JSON.stringify(generator.toJSON()); }
    };
};
...
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.toString"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>toString ()](#apidoc.element.uglifyjs.Buffer.prototype.toString)
- description and source-code
```javascript
toString = function () {
  let result;
  if (arguments.length === 0) {
    result = this.utf8Slice(0, this.length);
  } else {
    result = slowToString.apply(this, arguments);
  }
  if (result === undefined)
    throw new Error('"toString()" failed');
  return result;
}
```
- example usage
```shell
...
It enables some transformations that *might* break code logic in certain
contrived cases, but should be fine for most code.  You might want to try it
on your own code, it should reduce the minified size.  Here's what happens
when this flag is on:

- 'new Array(1, 2, 3)' or 'Array(1, 2, 3)' → '[1, 2, 3 ]'
- 'new Object()' → '{}'
- 'String(exp)' or 'exp.toString()' → '"" + exp'
- 'new Object/RegExp/Function/Error/Array (...)' → we discard the 'new'
- 'typeof foo == "undefined"' → 'foo === void 0'
- 'void 0' → 'undefined' (if there is a variable named "undefined" in
  scope; we do it because the variable name will be mangled, typically
  reduced to a single character).

### Conditional compilation
...
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.ucs2Slice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.ucs2Slice)
- description and source-code
```javascript
function ucs2Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.ucs2Write"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.uglifyjs.Buffer.prototype.ucs2Write)
- description and source-code
```javascript
function ucs2Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.utf8Slice"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.uglifyjs.Buffer.prototype.utf8Slice)
- description and source-code
```javascript
function utf8Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.utf8Write"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>utf8Write ()](#apidoc.element.uglifyjs.Buffer.prototype.utf8Write)
- description and source-code
```javascript
function utf8Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.write"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.uglifyjs.Buffer.prototype.write)
- description and source-code
```javascript
write = function (string, offset, length, encoding) {
  // Buffer#write(string);
  if (offset === undefined) {
    encoding = 'utf8';
    length = this.length;
    offset = 0;

  // Buffer#write(string, encoding)
  } else if (length === undefined && typeof offset === 'string') {
    encoding = offset;
    length = this.length;
    offset = 0;

  // Buffer#write(string, offset[, length][, encoding])
  } else if (isFinite(offset)) {
    offset = offset >>> 0;
    if (isFinite(length)) {
      length = length >>> 0;
      if (encoding === undefined)
        encoding = 'utf8';
    } else {
      encoding = length;
      length = undefined;
    }
  } else {
    // if someone is still calling the obsolete form of write(), tell them.
    // we don't want eg buf.write("foo", "utf8", 10) to silently turn into
    // buf.write("foo", "utf8"), so we can't ignore extra args
    throw new Error('Buffer.write(string, encoding, offset[, length]) ' +
                    'is no longer supported');
  }

  var remaining = this.length - offset;
  if (length === undefined || length > remaining)
    length = remaining;

  if (string.length > 0 && (length < 0 || offset < 0))
    throw new RangeError('Attempt to write outside buffer bounds');

  if (!encoding)
    encoding = 'utf8';

  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'hex':
        return this.hexWrite(string, offset, length);

      case 'utf8':
      case 'utf-8':
        return this.utf8Write(string, offset, length);

      case 'ascii':
        return this.asciiWrite(string, offset, length);

      case 'latin1':
      case 'binary':
        return this.latin1Write(string, offset, length);

      case 'base64':
        // Warning: maxLength not taken into account in base64Write
        return this.base64Write(string, offset, length);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return this.ucs2Write(string, offset, length);

      default:
        if (loweredCase)
          throw new TypeError('Unknown encoding: ' + encoding);
        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeDoubleBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeDoubleBE)
- description and source-code
```javascript
function writeDoubleBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleBE(this, val, offset);
  else
    binding.writeDoubleBE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeDoubleLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeDoubleLE)
- description and source-code
```javascript
function writeDoubleLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleLE(this, val, offset);
  else
    binding.writeDoubleLE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeFloatBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeFloatBE)
- description and source-code
```javascript
function writeFloatBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatBE(this, val, offset);
  else
    binding.writeFloatBE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeFloatLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeFloatLE)
- description and source-code
```javascript
function writeFloatLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatLE(this, val, offset);
  else
    binding.writeFloatLE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeInt16BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt16BE)
- description and source-code
```javascript
writeInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeInt16LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt16LE)
- description and source-code
```javascript
writeInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeInt32BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt32BE)
- description and source-code
```javascript
writeInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeInt32LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt32LE)
- description and source-code
```javascript
writeInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  this[offset + 2] = (value >>> 16);
  this[offset + 3] = (value >>> 24);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeInt8"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeInt8)
- description and source-code
```javascript
writeInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0x7f, -0x80);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeIntBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeIntBE)
- description and source-code
```javascript
writeIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = byteLength - 1;
  var mul = 1;
  var sub = 0;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i + 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeIntLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeIntLE)
- description and source-code
```javascript
writeIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = 0;
  var mul = 1;
  var sub = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i - 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUInt16BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt16BE)
- description and source-code
```javascript
writeUInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUInt16LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt16LE)
- description and source-code
```javascript
writeUInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUInt32BE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt32BE)
- description and source-code
```javascript
writeUInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUInt32LE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt32LE)
- description and source-code
```javascript
writeUInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset + 3] = (value >>> 24);
  this[offset + 2] = (value >>> 16);
  this[offset + 1] = (value >>> 8);
  this[offset] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUInt8"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUInt8)
- description and source-code
```javascript
writeUInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0xff, 0);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUIntBE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUIntBE)
- description and source-code
```javascript
writeUIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var i = byteLength - 1;
  var mul = 1;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Buffer.prototype.writeUIntLE"></a>[function <span class="apidocSignatureSpan">uglifyjs.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.uglifyjs.Buffer.prototype.writeUIntLE)
- description and source-code
```javascript
writeUIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var mul = 1;
  var i = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.Compressor"></a>[module uglifyjs.Compressor](#apidoc.module.uglifyjs.Compressor)

#### <a name="apidoc.element.uglifyjs.Compressor.Compressor"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>Compressor (options, false_by_default)](#apidoc.element.uglifyjs.Compressor.Compressor)
- description and source-code
```javascript
function Compressor(options, false_by_default) {
    if (!(this instanceof Compressor))
        return new Compressor(options, false_by_default);
    TreeTransformer.call(this, this.before, this.after);
    this.options = defaults(options, {
        sequences     : !false_by_default,
        properties    : !false_by_default,
        dead_code     : !false_by_default,
        drop_debugger : !false_by_default,
        unsafe        : false,
        unsafe_comps  : false,
        conditionals  : !false_by_default,
        comparisons   : !false_by_default,
        evaluate      : !false_by_default,
        booleans      : !false_by_default,
        loops         : !false_by_default,
        unused        : !false_by_default,
        hoist_funs    : !false_by_default,
        keep_fargs    : false,
        keep_fnames   : false,
        hoist_vars    : false,
        if_return     : !false_by_default,
        join_vars     : !false_by_default,
        cascade       : !false_by_default,
        side_effects  : !false_by_default,
        pure_getters  : false,
        pure_funcs    : null,
        negate_iife   : !false_by_default,
        screw_ie8     : false,
        drop_console  : false,
        angular       : false,

        warnings      : true,
        global_defs   : {}
    }, true);
}
```
- example usage
```shell
...
'''javascript
function uglify(ast, options, mangle) {
// Conversion from SpiderMonkey AST to internal format
var uAST = UglifyJS.AST_Node.from_mozilla_ast(ast);

// Compression
uAST.figure_out_scope();
uAST = uAST.transform(UglifyJS.Compressor(options));

// Mangling (optional)
if (mangle) {
  uAST.figure_out_scope();
  uAST.compute_char_frequency();
  uAST.mangle_names();
}
...
```



# <a name="apidoc.module.uglifyjs.Compressor.prototype"></a>[module uglifyjs.Compressor.prototype](#apidoc.module.uglifyjs.Compressor.prototype)

#### <a name="apidoc.element.uglifyjs.Compressor.prototype.before"></a>[function <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>before (node, descend, in_list)](#apidoc.element.uglifyjs.Compressor.prototype.before)
- description and source-code
```javascript
before = function (node, descend, in_list) {
    if (node._squeezed) return node;
    var was_scope = false;
    if (node instanceof AST_Scope) {
        node = node.hoist_declarations(this);
        was_scope = true;
    }
    descend(node, this);
    node = node.optimize(this);
    if (was_scope && node instanceof AST_Scope) {
        node.drop_unused(this);
        descend(node, this);
    }
    node._squeezed = true;
    return node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Compressor.prototype.option"></a>[function <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>option (key)](#apidoc.element.uglifyjs.Compressor.prototype.option)
- description and source-code
```javascript
option = function (key) { return this.options[key] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Compressor.prototype.warn"></a>[function <span class="apidocSignatureSpan">uglifyjs.Compressor.prototype.</span>warn ()](#apidoc.element.uglifyjs.Compressor.prototype.warn)
- description and source-code
```javascript
warn = function () {
    if (this.options.warnings)
        AST_Node.warn.apply(AST_Node, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.DefaultsError"></a>[module uglifyjs.DefaultsError](#apidoc.module.uglifyjs.DefaultsError)

#### <a name="apidoc.element.uglifyjs.DefaultsError.DefaultsError"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>DefaultsError (msg, defs)](#apidoc.element.uglifyjs.DefaultsError.DefaultsError)
- description and source-code
```javascript
function DefaultsError(msg, defs) {
    Error.call(this, msg);
    this.msg = msg;
    this.defs = defs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.DefaultsError.croak"></a>[function <span class="apidocSignatureSpan">uglifyjs.DefaultsError.</span>croak (msg, defs)](#apidoc.element.uglifyjs.DefaultsError.croak)
- description and source-code
```javascript
croak = function (msg, defs) {
    throw new DefaultsError(msg, defs);
}
```
- example usage
```shell
...
};

function defaults(args, defs, croak) {
    if (args === true)
        args = {};
    var ret = args || {};
    if (croak) for (var i in ret) if (ret.hasOwnProperty(i) && !defs.hasOwnProperty(i))
        DefaultsError.croak("'" + i + "' is not a supported option", defs);
    for (var i in defs) if (defs.hasOwnProperty(i)) {
        ret[i] = (args && args.hasOwnProperty(i)) ? args[i] : defs[i];
    }
    return ret;
};

function merge(obj, ext) {
...
```



# <a name="apidoc.module.uglifyjs.DefaultsError.prototype"></a>[module uglifyjs.DefaultsError.prototype](#apidoc.module.uglifyjs.DefaultsError.prototype)

#### <a name="apidoc.element.uglifyjs.DefaultsError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">uglifyjs.DefaultsError.prototype.</span>constructor (msg, defs)](#apidoc.element.uglifyjs.DefaultsError.prototype.constructor)
- description and source-code
```javascript
function DefaultsError(msg, defs) {
    Error.call(this, msg);
    this.msg = msg;
    this.defs = defs;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.Dictionary"></a>[module uglifyjs.Dictionary](#apidoc.module.uglifyjs.Dictionary)

#### <a name="apidoc.element.uglifyjs.Dictionary.Dictionary"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>Dictionary ()](#apidoc.element.uglifyjs.Dictionary.Dictionary)
- description and source-code
```javascript
function Dictionary() {
    this._values = Object.create(null);
    this._size = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.Dictionary.prototype"></a>[module uglifyjs.Dictionary.prototype](#apidoc.module.uglifyjs.Dictionary.prototype)

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.add"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>add (key, val)](#apidoc.element.uglifyjs.Dictionary.prototype.add)
- description and source-code
```javascript
add = function (key, val) {
    if (this.has(key)) {
        this.get(key).push(val);
    } else {
        this.set(key, [ val ]);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.del"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>del (key)](#apidoc.element.uglifyjs.Dictionary.prototype.del)
- description and source-code
```javascript
del = function (key) {
    if (this.has(key)) {
        --this._size;
        delete this._values["$" + key];
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.each"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>each (f)](#apidoc.element.uglifyjs.Dictionary.prototype.each)
- description and source-code
```javascript
each = function (f) {
    for (var i in this._values)
        f(this._values[i], i.substr(1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.get"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>get (key)](#apidoc.element.uglifyjs.Dictionary.prototype.get)
- description and source-code
```javascript
get = function (key) { return this._values["$" + key] }
```
- example usage
```shell
...
set: function(key, val) {
    if (!this.has(key)) ++this._size;
    this._values["$" + key] = val;
    return this;
},
add: function(key, val) {
    if (this.has(key)) {
        this.get(key).push(val);
    } else {
        this.set(key, [ val ]);
    }
    return this;
},
get: function(key) { return this._values["$" + key] },
del: function(key) {
...
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.has"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>has (key)](#apidoc.element.uglifyjs.Dictionary.prototype.has)
- description and source-code
```javascript
has = function (key) { return ("$" + key) in this._values }
```
- example usage
```shell
...

function Dictionary() {
this._values = Object.create(null);
this._size = 0;
};
Dictionary.prototype = {
set: function(key, val) {
    if (!this.has(key)) ++this._size;
    this._values["$" + key] = val;
    return this;
},
add: function(key, val) {
    if (this.has(key)) {
        this.get(key).push(val);
    } else {
...
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.map"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>map (f)](#apidoc.element.uglifyjs.Dictionary.prototype.map)
- description and source-code
```javascript
map = function (f) {
    var ret = [];
    for (var i in this._values)
        ret.push(f(this._values[i], i.substr(1)));
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.set"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>set (key, val)](#apidoc.element.uglifyjs.Dictionary.prototype.set)
- description and source-code
```javascript
set = function (key, val) {
    if (!this.has(key)) ++this._size;
    this._values["$" + key] = val;
    return this;
}
```
- example usage
```shell
...
    this._values["$" + key] = val;
    return this;
},
add: function(key, val) {
    if (this.has(key)) {
        this.get(key).push(val);
    } else {
        this.set(key, [ val ]);
    }
    return this;
},
get: function(key) { return this._values["$" + key] },
del: function(key) {
    if (this.has(key)) {
        --this._size;
...
```

#### <a name="apidoc.element.uglifyjs.Dictionary.prototype.size"></a>[function <span class="apidocSignatureSpan">uglifyjs.Dictionary.prototype.</span>size ()](#apidoc.element.uglifyjs.Dictionary.prototype.size)
- description and source-code
```javascript
size = function () {
    return this._size;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.JS_Parse_Error"></a>[module uglifyjs.JS_Parse_Error](#apidoc.module.uglifyjs.JS_Parse_Error)

#### <a name="apidoc.element.uglifyjs.JS_Parse_Error.JS_Parse_Error"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>JS_Parse_Error (message, filename, line, col, pos)](#apidoc.element.uglifyjs.JS_Parse_Error.JS_Parse_Error)
- description and source-code
```javascript
function JS_Parse_Error(message, filename, line, col, pos) {
    this.message = message;
    this.filename = filename;
    this.line = line;
    this.col = col;
    this.pos = pos;
    this.stack = new Error().stack;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.JS_Parse_Error.prototype"></a>[module uglifyjs.JS_Parse_Error.prototype](#apidoc.module.uglifyjs.JS_Parse_Error.prototype)

#### <a name="apidoc.element.uglifyjs.JS_Parse_Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">uglifyjs.JS_Parse_Error.prototype.</span>toString ()](#apidoc.element.uglifyjs.JS_Parse_Error.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return this.message + " (line: " + this.line + ", col: " + this.col + ", pos: " + this.pos + ")" + "\n\n" + this.stack;
}
```
- example usage
```shell
...
It enables some transformations that *might* break code logic in certain
contrived cases, but should be fine for most code.  You might want to try it
on your own code, it should reduce the minified size.  Here's what happens
when this flag is on:

- 'new Array(1, 2, 3)' or 'Array(1, 2, 3)' → '[1, 2, 3 ]'
- 'new Object()' → '{}'
- 'String(exp)' or 'exp.toString()' → '"" + exp'
- 'new Object/RegExp/Function/Error/Array (...)' → we discard the 'new'
- 'typeof foo == "undefined"' → 'foo === void 0'
- 'void 0' → 'undefined' (if there is a variable named "undefined" in
  scope; we do it because the variable name will be mangled, typically
  reduced to a single character).

### Conditional compilation
...
```



# <a name="apidoc.module.uglifyjs.MAP"></a>[module uglifyjs.MAP](#apidoc.module.uglifyjs.MAP)

#### <a name="apidoc.element.uglifyjs.MAP.MAP"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>MAP (a, f, backwards)](#apidoc.element.uglifyjs.MAP.MAP)
- description and source-code
```javascript
function MAP(a, f, backwards) {
    var ret = [], top = [], i;
    function doit() {
        var val = f(a[i], i);
        var is_last = val instanceof Last;
        if (is_last) val = val.v;
        if (val instanceof AtTop) {
            val = val.v;
            if (val instanceof Splice) {
                top.push.apply(top, backwards ? val.v.slice().reverse() : val.v);
            } else {
                top.push(val);
            }
        }
        else if (val !== skip) {
            if (val instanceof Splice) {
                ret.push.apply(ret, backwards ? val.v.slice().reverse() : val.v);
            } else {
                ret.push(val);
            }
        }
        return is_last;
    };
    if (a instanceof Array) {
        if (backwards) {
            for (i = a.length; --i >= 0;) if (doit()) break;
            ret.reverse();
            top.reverse();
        } else {
            for (i = 0; i < a.length; ++i) if (doit()) break;
        }
    }
    else {
        for (i in a) if (a.hasOwnProperty(i)) if (doit()) break;
    }
    return top.concat(ret);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MAP.at_top"></a>[function <span class="apidocSignatureSpan">uglifyjs.MAP.</span>at_top (val)](#apidoc.element.uglifyjs.MAP.at_top)
- description and source-code
```javascript
at_top = function (val) { return new AtTop(val) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MAP.last"></a>[function <span class="apidocSignatureSpan">uglifyjs.MAP.</span>last (val)](#apidoc.element.uglifyjs.MAP.last)
- description and source-code
```javascript
last = function (val) { return new Last(val) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MAP.splice"></a>[function <span class="apidocSignatureSpan">uglifyjs.MAP.</span>splice (val)](#apidoc.element.uglifyjs.MAP.splice)
- description and source-code
```javascript
splice = function (val) { return new Splice(val) }
```
- example usage
```shell
...
        parameters.push(pair.substr(splitAt + 1));
    });

    var wrapped_tl = "(function(" + parameters.join(",") + "){ '$ORIG'; })(" + args.join(",") + ")";
    wrapped_tl = parse(wrapped_tl);
    wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
        if (node instanceof AST_Directive && node.value == "$ORIG") {
            return MAP.splice(self.body);
        }
    }));
    return wrapped_tl;
},
wrap_commonjs: function(name, export_all) {
    var self = this;
    var to_export = [];
...
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap"></a>[module uglifyjs.MOZ_SourceMap](#apidoc.module.uglifyjs.MOZ_SourceMap)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapConsumer (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer)
- description and source-code
```javascript
function SourceMapConsumer(aSourceMap) {
  var sourceMap = aSourceMap;
  if (typeof aSourceMap === 'string') {
    sourceMap = JSON.parse(aSourceMap.replace(/^\)\]\}'/, ''));
  }

  var version = util.getArg(sourceMap, 'version');
  var sources = util.getArg(sourceMap, 'sources');
  // Sass 3.3 leaves out the 'names' array, so we deviate from the spec (which
  // requires the array) to play nice here.
  var names = util.getArg(sourceMap, 'names', []);
  var sourceRoot = util.getArg(sourceMap, 'sourceRoot', null);
  var sourcesContent = util.getArg(sourceMap, 'sourcesContent', null);
  var mappings = util.getArg(sourceMap, 'mappings');
  var file = util.getArg(sourceMap, 'file', null);

  // Once again, Sass deviates from the spec and supplies the version as a
  // string rather than a number, so we use loose equality checking here.
  if (version != this._version) {
    throw new Error('Unsupported version: ' + version);
  }

  // Pass 'true' below to allow duplicate names and sources. While source maps
  // are intended to be compressed and deduplicated, the TypeScript compiler
  // sometimes generates source maps with duplicates in them. See Github issue
  // #72 and bugzil.la/889492.
  this._names = ArraySet.fromArray(names, true);
  this._sources = ArraySet.fromArray(sources, true);

  this.sourceRoot = sourceRoot;
  this.sourcesContent = sourcesContent;
  this._mappings = mappings;
  this.file = file;
}
```
- example usage
```shell
...
    file : null,
    root : null,
    orig : null,

    orig_line_diff : 0,
    dest_line_diff : 0,
});
var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
var generator;
if (orig_map) {
  generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
} else {
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapGenerator (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator)
- description and source-code
```javascript
function SourceMapGenerator(aArgs) {
  if (!aArgs) {
    aArgs = {};
  }
  this._file = util.getArg(aArgs, 'file', null);
  this._sourceRoot = util.getArg(aArgs, 'sourceRoot', null);
  this._sources = new ArraySet();
  this._names = new ArraySet();
  this._mappings = [];
  this._sourcesContents = null;
}
```
- example usage
```shell
...
    dest_line_diff : 0,
});
var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
var generator;
if (orig_map) {
  generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
} else {
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
    });
}
function add(source, gen_line, gen_col, orig_line, orig_col, name) {
    if (orig_map) {
        var info = orig_map.originalPositionFor({
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceNode (aLine, aColumn, aSource, aChunks, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode)
- description and source-code
```javascript
function SourceNode(aLine, aColumn, aSource, aChunks, aName) {
  this.children = [];
  this.sourceContents = {};
  this.line = aLine === undefined ? null : aLine;
  this.column = aColumn === undefined ? null : aColumn;
  this.source = aSource === undefined ? null : aSource;
  this.name = aName === undefined ? null : aName;
  if (aChunks != null) this.add(aChunks);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapConsumer"></a>[module uglifyjs.MOZ_SourceMap.SourceMapConsumer](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapConsumer)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.SourceMapConsumer"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapConsumer (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.SourceMapConsumer)
- description and source-code
```javascript
function SourceMapConsumer(aSourceMap) {
  var sourceMap = aSourceMap;
  if (typeof aSourceMap === 'string') {
    sourceMap = JSON.parse(aSourceMap.replace(/^\)\]\}'/, ''));
  }

  var version = util.getArg(sourceMap, 'version');
  var sources = util.getArg(sourceMap, 'sources');
  // Sass 3.3 leaves out the 'names' array, so we deviate from the spec (which
  // requires the array) to play nice here.
  var names = util.getArg(sourceMap, 'names', []);
  var sourceRoot = util.getArg(sourceMap, 'sourceRoot', null);
  var sourcesContent = util.getArg(sourceMap, 'sourcesContent', null);
  var mappings = util.getArg(sourceMap, 'mappings');
  var file = util.getArg(sourceMap, 'file', null);

  // Once again, Sass deviates from the spec and supplies the version as a
  // string rather than a number, so we use loose equality checking here.
  if (version != this._version) {
    throw new Error('Unsupported version: ' + version);
  }

  // Pass 'true' below to allow duplicate names and sources. While source maps
  // are intended to be compressed and deduplicated, the TypeScript compiler
  // sometimes generates source maps with duplicates in them. See Github issue
  // #72 and bugzil.la/889492.
  this._names = ArraySet.fromArray(names, true);
  this._sources = ArraySet.fromArray(sources, true);

  this.sourceRoot = sourceRoot;
  this.sourcesContent = sourcesContent;
  this._mappings = mappings;
  this.file = file;
}
```
- example usage
```shell
...
    file : null,
    root : null,
    orig : null,

    orig_line_diff : 0,
    dest_line_diff : 0,
});
var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
var generator;
if (orig_map) {
  generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
} else {
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.fromSourceMap"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.</span>fromSourceMap (aSourceMap)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.fromSourceMap)
- description and source-code
```javascript
function SourceMapConsumer_fromSourceMap(aSourceMap) {
  var smc = Object.create(SourceMapConsumer.prototype);

  smc._names = ArraySet.fromArray(aSourceMap._names.toArray(), true);
  smc._sources = ArraySet.fromArray(aSourceMap._sources.toArray(), true);
  smc.sourceRoot = aSourceMap._sourceRoot;
  smc.sourcesContent = aSourceMap._generateSourcesContent(smc._sources.toArray(),
                                                          smc.sourceRoot);
  smc.file = aSourceMap._file;

  smc.__generatedMappings = aSourceMap._mappings.slice()
    .sort(util.compareByGeneratedPositions);
  smc.__originalMappings = aSourceMap._mappings.slice()
    .sort(util.compareByOriginalPositions);

  return smc;
}
```
- example usage
```shell
...

    orig_line_diff : 0,
    dest_line_diff : 0,
});
var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
var generator;
if (orig_map) {
  generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
} else {
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
    });
}
function add(source, gen_line, gen_col, orig_line, orig_col, name) {
...
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype"></a>[module uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype._findMapping"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>_findMapping (aNeedle, aMappings, aLineName, aColumnName, aComparator)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype._findMapping)
- description and source-code
```javascript
function SourceMapConsumer_findMapping(aNeedle, aMappings, aLineName, aColumnName, aComparator) {
  // To return the position we are searching for, we must first find the
  // mapping for the given position and then return the opposite position it
  // points to. Because the mappings are sorted, we can use binary search to
  // find the best mapping.

  if (aNeedle[aLineName] <= 0) {
    throw new TypeError('Line must be greater than or equal to 1, got '
                        + aNeedle[aLineName]);
  }
  if (aNeedle[aColumnName] < 0) {
    throw new TypeError('Column must be greater than or equal to 0, got '
                        + aNeedle[aColumnName]);
  }

  return binarySearch.search(aNeedle, aMappings, aComparator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype._parseMappings"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>_parseMappings (aStr, aSourceRoot)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype._parseMappings)
- description and source-code
```javascript
function SourceMapConsumer_parseMappings(aStr, aSourceRoot) {
  var generatedLine = 1;
  var previousGeneratedColumn = 0;
  var previousOriginalLine = 0;
  var previousOriginalColumn = 0;
  var previousSource = 0;
  var previousName = 0;
  var mappingSeparator = /^[,;]/;
  var str = aStr;
  var mapping;
  var temp;

  while (str.length > 0) {
    if (str.charAt(0) === ';') {
      generatedLine++;
      str = str.slice(1);
      previousGeneratedColumn = 0;
    }
    else if (str.charAt(0) === ',') {
      str = str.slice(1);
    }
    else {
      mapping = {};
      mapping.generatedLine = generatedLine;

      // Generated column.
      temp = base64VLQ.decode(str);
      mapping.generatedColumn = previousGeneratedColumn + temp.value;
      previousGeneratedColumn = mapping.generatedColumn;
      str = temp.rest;

      if (str.length > 0 && !mappingSeparator.test(str.charAt(0))) {
        // Original source.
        temp = base64VLQ.decode(str);
        mapping.source = this._sources.at(previousSource + temp.value);
        previousSource += temp.value;
        str = temp.rest;
        if (str.length === 0 || mappingSeparator.test(str.charAt(0))) {
          throw new Error('Found a source, but no line and column');
        }

        // Original line.
        temp = base64VLQ.decode(str);
        mapping.originalLine = previousOriginalLine + temp.value;
        previousOriginalLine = mapping.originalLine;
        // Lines are stored 0-based
        mapping.originalLine += 1;
        str = temp.rest;
        if (str.length === 0 || mappingSeparator.test(str.charAt(0))) {
          throw new Error('Found a source and line, but no column');
        }

        // Original column.
        temp = base64VLQ.decode(str);
        mapping.originalColumn = previousOriginalColumn + temp.value;
        previousOriginalColumn = mapping.originalColumn;
        str = temp.rest;

        if (str.length > 0 && !mappingSeparator.test(str.charAt(0))) {
          // Original name.
          temp = base64VLQ.decode(str);
          mapping.name = this._names.at(previousName + temp.value);
          previousName += temp.value;
          str = temp.rest;
        }
      }

      this.__generatedMappings.push(mapping);
      if (typeof mapping.originalLine === 'number') {
        this.__originalMappings.push(mapping);
      }
    }
  }

  this.__generatedMappings.sort(util.compareByGeneratedPositions);
  this.__originalMappings.sort(util.compareByOriginalPositions);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.eachMapping"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>eachMapping (aCallback, aContext, aOrder)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.eachMapping)
- description and source-code
```javascript
function SourceMapConsumer_eachMapping(aCallback, aContext, aOrder) {
  var context = aContext || null;
  var order = aOrder || SourceMapConsumer.GENERATED_ORDER;

  var mappings;
  switch (order) {
  case SourceMapConsumer.GENERATED_ORDER:
    mappings = this._generatedMappings;
    break;
  case SourceMapConsumer.ORIGINAL_ORDER:
    mappings = this._originalMappings;
    break;
  default:
    throw new Error("Unknown order of iteration.");
  }

  var sourceRoot = this.sourceRoot;
  mappings.map(function (mapping) {
    var source = mapping.source;
    if (source && sourceRoot) {
      source = util.join(sourceRoot, source);
    }
    return {
      source: source,
      generatedLine: mapping.generatedLine,
      generatedColumn: mapping.generatedColumn,
      originalLine: mapping.originalLine,
      originalColumn: mapping.originalColumn,
      name: mapping.name
    };
  }).forEach(aCallback, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.generatedPositionFor"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>generatedPositionFor (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.generatedPositionFor)
- description and source-code
```javascript
function SourceMapConsumer_generatedPositionFor(aArgs) {
  var needle = {
    source: util.getArg(aArgs, 'source'),
    originalLine: util.getArg(aArgs, 'line'),
    originalColumn: util.getArg(aArgs, 'column')
  };

  if (this.sourceRoot) {
    needle.source = util.relative(this.sourceRoot, needle.source);
  }

  var mapping = this._findMapping(needle,
                                  this._originalMappings,
                                  "originalLine",
                                  "originalColumn",
                                  util.compareByOriginalPositions);

  if (mapping) {
    return {
      line: util.getArg(mapping, 'generatedLine', null),
      column: util.getArg(mapping, 'generatedColumn', null)
    };
  }

  return {
    line: null,
    column: null
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.originalPositionFor"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>originalPositionFor (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.originalPositionFor)
- description and source-code
```javascript
function SourceMapConsumer_originalPositionFor(aArgs) {
  var needle = {
    generatedLine: util.getArg(aArgs, 'line'),
    generatedColumn: util.getArg(aArgs, 'column')
  };

  var mapping = this._findMapping(needle,
                                  this._generatedMappings,
                                  "generatedLine",
                                  "generatedColumn",
                                  util.compareByGeneratedPositions);

  if (mapping && mapping.generatedLine === needle.generatedLine) {
    var source = util.getArg(mapping, 'source', null);
    if (source && this.sourceRoot) {
      source = util.join(this.sourceRoot, source);
    }
    return {
      source: source,
      line: util.getArg(mapping, 'originalLine', null),
      column: util.getArg(mapping, 'originalColumn', null),
      name: util.getArg(mapping, 'name', null)
    };
  }

  return {
    source: null,
    line: null,
    column: null,
    name: null
  };
}
```
- example usage
```shell
...
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
    });
}
function add(source, gen_line, gen_col, orig_line, orig_col, name) {
    if (orig_map) {
        var info = orig_map.originalPositionFor({
            line: orig_line,
            column: orig_col
        });
        if (info.source === null) {
            return;
        }
        source = info.source;
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.sourceContentFor"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.</span>sourceContentFor (aSource)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapConsumer.prototype.sourceContentFor)
- description and source-code
```javascript
function SourceMapConsumer_sourceContentFor(aSource) {
  if (!this.sourcesContent) {
    return null;
  }

  if (this.sourceRoot) {
    aSource = util.relative(this.sourceRoot, aSource);
  }

  if (this._sources.has(aSource)) {
    return this.sourcesContent[this._sources.indexOf(aSource)];
  }

  var url;
  if (this.sourceRoot
      && (url = util.urlParse(this.sourceRoot))) {
    // XXX: file:// URIs and absolute paths lead to unexpected behavior for
    // many users. We can help them out when they expect file:// URIs to
    // behave like it would if they were running a local HTTP server. See
    // https://bugzilla.mozilla.org/show_bug.cgi?id=885597.
    var fileUriAbsPath = aSource.replace(/^file:\/\//, "");
    if (url.scheme == "file"
        && this._sources.has(fileUriAbsPath)) {
      return this.sourcesContent[this._sources.indexOf(fileUriAbsPath)]
    }

    if ((!url.path || url.path == "/")
        && this._sources.has("/" + aSource)) {
      return this.sourcesContent[this._sources.indexOf("/" + aSource)];
    }
  }

  throw new Error('"' + aSource + '" is not in the SourceMap.');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapGenerator"></a>[module uglifyjs.MOZ_SourceMap.SourceMapGenerator](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapGenerator)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.SourceMapGenerator"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceMapGenerator (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.SourceMapGenerator)
- description and source-code
```javascript
function SourceMapGenerator(aArgs) {
  if (!aArgs) {
    aArgs = {};
  }
  this._file = util.getArg(aArgs, 'file', null);
  this._sourceRoot = util.getArg(aArgs, 'sourceRoot', null);
  this._sources = new ArraySet();
  this._names = new ArraySet();
  this._mappings = [];
  this._sourcesContents = null;
}
```
- example usage
```shell
...
    dest_line_diff : 0,
});
var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
var generator;
if (orig_map) {
  generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
} else {
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
    });
}
function add(source, gen_line, gen_col, orig_line, orig_col, name) {
    if (orig_map) {
        var info = orig_map.originalPositionFor({
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.fromSourceMap"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.</span>fromSourceMap (aSourceMapConsumer)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.fromSourceMap)
- description and source-code
```javascript
function SourceMapGenerator_fromSourceMap(aSourceMapConsumer) {
  var sourceRoot = aSourceMapConsumer.sourceRoot;
  var generator = new SourceMapGenerator({
    file: aSourceMapConsumer.file,
    sourceRoot: sourceRoot
  });
  aSourceMapConsumer.eachMapping(function (mapping) {
    var newMapping = {
      generated: {
        line: mapping.generatedLine,
        column: mapping.generatedColumn
      }
    };

    if (mapping.source) {
      newMapping.source = mapping.source;
      if (sourceRoot) {
        newMapping.source = util.relative(sourceRoot, newMapping.source);
      }

      newMapping.original = {
        line: mapping.originalLine,
        column: mapping.originalColumn
      };

      if (mapping.name) {
        newMapping.name = mapping.name;
      }
    }

    generator.addMapping(newMapping);
  });
  aSourceMapConsumer.sources.forEach(function (sourceFile) {
    var content = aSourceMapConsumer.sourceContentFor(sourceFile);
    if (content) {
      generator.setSourceContent(sourceFile, content);
    }
  });
  return generator;
}
```
- example usage
```shell
...

    orig_line_diff : 0,
    dest_line_diff : 0,
});
var orig_map = options.orig && new MOZ_SourceMap.SourceMapConsumer(options.orig);
var generator;
if (orig_map) {
  generator = MOZ_SourceMap.SourceMapGenerator.fromSourceMap(orig_map);
} else {
    generator = new MOZ_SourceMap.SourceMapGenerator({
        file       : options.file,
        sourceRoot : options.root
    });
}
function add(source, gen_line, gen_col, orig_line, orig_col, name) {
...
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype"></a>[module uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._generateSourcesContent"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_generateSourcesContent (aSources, aSourceRoot)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._generateSourcesContent)
- description and source-code
```javascript
function SourceMapGenerator_generateSourcesContent(aSources, aSourceRoot) {
  return aSources.map(function (source) {
    if (!this._sourcesContents) {
      return null;
    }
    if (aSourceRoot) {
      source = util.relative(aSourceRoot, source);
    }
    var key = util.toSetString(source);
    return Object.prototype.hasOwnProperty.call(this._sourcesContents,
                                                key)
      ? this._sourcesContents[key]
      : null;
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._serializeMappings"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_serializeMappings ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._serializeMappings)
- description and source-code
```javascript
function SourceMapGenerator_serializeMappings() {
  var previousGeneratedColumn = 0;
  var previousGeneratedLine = 1;
  var previousOriginalColumn = 0;
  var previousOriginalLine = 0;
  var previousName = 0;
  var previousSource = 0;
  var result = '';
  var mapping;

  // The mappings must be guaranteed to be in sorted order before we start
  // serializing them or else the generated line numbers (which are defined
  // via the ';' separators) will be all messed up. Note: it might be more
  // performant to maintain the sorting as we insert them, rather than as we
  // serialize them, but the big O is the same either way.
  this._mappings.sort(util.compareByGeneratedPositions);

  for (var i = 0, len = this._mappings.length; i < len; i++) {
    mapping = this._mappings[i];

    if (mapping.generatedLine !== previousGeneratedLine) {
      previousGeneratedColumn = 0;
      while (mapping.generatedLine !== previousGeneratedLine) {
        result += ';';
        previousGeneratedLine++;
      }
    }
    else {
      if (i > 0) {
        if (!util.compareByGeneratedPositions(mapping, this._mappings[i - 1])) {
          continue;
        }
        result += ',';
      }
    }

    result += base64VLQ.encode(mapping.generatedColumn
                               - previousGeneratedColumn);
    previousGeneratedColumn = mapping.generatedColumn;

    if (mapping.source) {
      result += base64VLQ.encode(this._sources.indexOf(mapping.source)
                                 - previousSource);
      previousSource = this._sources.indexOf(mapping.source);

      // lines are stored 0-based in SourceMap spec version 3
      result += base64VLQ.encode(mapping.originalLine - 1
                                 - previousOriginalLine);
      previousOriginalLine = mapping.originalLine - 1;

      result += base64VLQ.encode(mapping.originalColumn
                                 - previousOriginalColumn);
      previousOriginalColumn = mapping.originalColumn;

      if (mapping.name) {
        result += base64VLQ.encode(this._names.indexOf(mapping.name)
                                   - previousName);
        previousName = this._names.indexOf(mapping.name);
      }
    }
  }

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._validateMapping"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>_validateMapping (aGenerated, aOriginal, aSource, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype._validateMapping)
- description and source-code
```javascript
function SourceMapGenerator_validateMapping(aGenerated, aOriginal, aSource, aName) {
  if (aGenerated && 'line' in aGenerated && 'column' in aGenerated
      && aGenerated.line > 0 && aGenerated.column >= 0
      && !aOriginal && !aSource && !aName) {
    // Case 1.
    return;
  }
  else if (aGenerated && 'line' in aGenerated && 'column' in aGenerated
           && aOriginal && 'line' in aOriginal && 'column' in aOriginal
           && aGenerated.line > 0 && aGenerated.column >= 0
           && aOriginal.line > 0 && aOriginal.column >= 0
           && aSource) {
    // Cases 2 and 3.
    return;
  }
  else {
    throw new Error('Invalid mapping: ' + JSON.stringify({
      generated: aGenerated,
      source: aSource,
      original: aOriginal,
      name: aName
    }));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.addMapping"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>addMapping (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.addMapping)
- description and source-code
```javascript
function SourceMapGenerator_addMapping(aArgs) {
  var generated = util.getArg(aArgs, 'generated');
  var original = util.getArg(aArgs, 'original', null);
  var source = util.getArg(aArgs, 'source', null);
  var name = util.getArg(aArgs, 'name', null);

  this._validateMapping(generated, original, source, name);

  if (source && !this._sources.has(source)) {
    this._sources.add(source);
  }

  if (name && !this._names.has(name)) {
    this._names.add(name);
  }

  this._mappings.push({
    generatedLine: generated.line,
    generatedColumn: generated.column,
    originalLine: original != null && original.line,
    originalColumn: original != null && original.column,
    source: source,
    name: name
  });
}
```
- example usage
```shell
...
            return;
        }
        source = info.source;
        orig_line = info.line;
        orig_col = info.column;
        name = info.name || name;
    }
    generator.addMapping({
        generated : { line: gen_line + options.dest_line_diff, column: gen_col },
        original  : { line: orig_line + options.orig_line_diff, column: orig_col },
        source    : source,
        name      : name
    });
}
return {
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.applySourceMap"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>applySourceMap (aSourceMapConsumer, aSourceFile, aSourceMapPath)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.applySourceMap)
- description and source-code
```javascript
function SourceMapGenerator_applySourceMap(aSourceMapConsumer, aSourceFile, aSourceMapPath) {
  // If aSourceFile is omitted, we will use the file property of the SourceMap
  if (!aSourceFile) {
    if (!aSourceMapConsumer.file) {
      throw new Error(
        'SourceMapGenerator.prototype.applySourceMap requires either an explicit source file, ' +
        'or the source map\'s "file" property. Both were omitted.'
      );
    }
    aSourceFile = aSourceMapConsumer.file;
  }
  var sourceRoot = this._sourceRoot;
  // Make "aSourceFile" relative if an absolute Url is passed.
  if (sourceRoot) {
    aSourceFile = util.relative(sourceRoot, aSourceFile);
  }
  // Applying the SourceMap can add and remove items from the sources and
  // the names array.
  var newSources = new ArraySet();
  var newNames = new ArraySet();

  // Find mappings for the "aSourceFile"
  this._mappings.forEach(function (mapping) {
    if (mapping.source === aSourceFile && mapping.originalLine) {
      // Check if it can be mapped by the source map, then update the mapping.
      var original = aSourceMapConsumer.originalPositionFor({
        line: mapping.originalLine,
        column: mapping.originalColumn
      });
      if (original.source !== null) {
        // Copy mapping
        mapping.source = original.source;
        if (aSourceMapPath) {
          mapping.source = util.join(aSourceMapPath, mapping.source)
        }
        if (sourceRoot) {
          mapping.source = util.relative(sourceRoot, mapping.source);
        }
        mapping.originalLine = original.line;
        mapping.originalColumn = original.column;
        if (original.name !== null && mapping.name !== null) {
          // Only use the identifier name if it's an identifier
          // in both SourceMaps
          mapping.name = original.name;
        }
      }
    }

    var source = mapping.source;
    if (source && !newSources.has(source)) {
      newSources.add(source);
    }

    var name = mapping.name;
    if (name && !newNames.has(name)) {
      newNames.add(name);
    }

  }, this);
  this._sources = newSources;
  this._names = newNames;

  // Copy sourcesContents of applied map.
  aSourceMapConsumer.sources.forEach(function (sourceFile) {
    var content = aSourceMapConsumer.sourceContentFor(sourceFile);
    if (content) {
      if (aSourceMapPath) {
        sourceFile = util.join(aSourceMapPath, sourceFile);
      }
      if (sourceRoot) {
        sourceFile = util.relative(sourceRoot, sourceFile);
      }
      this.setSourceContent(sourceFile, content);
    }
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.setSourceContent"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>setSourceContent (aSourceFile, aSourceContent)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.setSourceContent)
- description and source-code
```javascript
function SourceMapGenerator_setSourceContent(aSourceFile, aSourceContent) {
  var source = aSourceFile;
  if (this._sourceRoot) {
    source = util.relative(this._sourceRoot, source);
  }

  if (aSourceContent !== null) {
    // Add the source content to the _sourcesContents map.
    // Create a new _sourcesContents map if the property is null.
    if (!this._sourcesContents) {
      this._sourcesContents = {};
    }
    this._sourcesContents[util.toSetString(source)] = aSourceContent;
  } else {
    // Remove the source file from the _sourcesContents map.
    // If the _sourcesContents map is empty, set the property to null.
    delete this._sourcesContents[util.toSetString(source)];
    if (Object.keys(this._sourcesContents).length === 0) {
      this._sourcesContents = null;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>toJSON ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.toJSON)
- description and source-code
```javascript
function SourceMapGenerator_toJSON() {
  var map = {
    version: this._version,
    file: this._file,
    sources: this._sources.toArray(),
    names: this._names.toArray(),
    mappings: this._serializeMappings()
  };
  if (this._sourceRoot) {
    map.sourceRoot = this._sourceRoot;
  }
  if (this._sourcesContents) {
    map.sourcesContent = this._generateSourcesContent(map.sources, map.sourceRoot);
  }

  return map;
}
```
- example usage
```shell
...
            source    : source,
            name      : name
        });
    }
    return {
        add        : add,
        get        : function() { return generator },
        toString   : function() { return JSON.stringify(generator.toJSON()); }
    };
};
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.toString"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.</span>toString ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceMapGenerator.prototype.toString)
- description and source-code
```javascript
function SourceMapGenerator_toString() {
  return JSON.stringify(this);
}
```
- example usage
```shell
...
It enables some transformations that *might* break code logic in certain
contrived cases, but should be fine for most code.  You might want to try it
on your own code, it should reduce the minified size.  Here's what happens
when this flag is on:

- 'new Array(1, 2, 3)' or 'Array(1, 2, 3)' → '[1, 2, 3 ]'
- 'new Object()' → '{}'
- 'String(exp)' or 'exp.toString()' → '"" + exp'
- 'new Object/RegExp/Function/Error/Array (...)' → we discard the 'new'
- 'typeof foo == "undefined"' → 'foo === void 0'
- 'void 0' → 'undefined' (if there is a variable named "undefined" in
  scope; we do it because the variable name will be mangled, typically
  reduced to a single character).

### Conditional compilation
...
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap.SourceNode"></a>[module uglifyjs.MOZ_SourceMap.SourceNode](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceNode)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.SourceNode"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.</span>SourceNode (aLine, aColumn, aSource, aChunks, aName)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.SourceNode)
- description and source-code
```javascript
function SourceNode(aLine, aColumn, aSource, aChunks, aName) {
  this.children = [];
  this.sourceContents = {};
  this.line = aLine === undefined ? null : aLine;
  this.column = aColumn === undefined ? null : aColumn;
  this.source = aSource === undefined ? null : aSource;
  this.name = aName === undefined ? null : aName;
  if (aChunks != null) this.add(aChunks);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.fromStringWithSourceMap"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.</span>fromStringWithSourceMap (aGeneratedCode, aSourceMapConsumer)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.fromStringWithSourceMap)
- description and source-code
```javascript
function SourceNode_fromStringWithSourceMap(aGeneratedCode, aSourceMapConsumer) {
  // The SourceNode we want to fill with the generated code
  // and the SourceMap
  var node = new SourceNode();

  // All even indices of this array are one line of the generated code,
  // while all odd indices are the newlines between two adjacent lines
  // (since 'REGEX_NEWLINE' captures its match).
  // Processed fragments are removed from this array, by calling 'shiftNextLine'.
  var remainingLines = aGeneratedCode.split(REGEX_NEWLINE);
  var shiftNextLine = function() {
    var lineContents = remainingLines.shift();
    // The last line of a file might not have a newline.
    var newLine = remainingLines.shift() || "";
    return lineContents + newLine;
  };

  // We need to remember the position of "remainingLines"
  var lastGeneratedLine = 1, lastGeneratedColumn = 0;

  // The generate SourceNodes we need a code range.
  // To extract it current and last mapping is used.
  // Here we store the last mapping.
  var lastMapping = null;

  aSourceMapConsumer.eachMapping(function (mapping) {
    if (lastMapping !== null) {
      // We add the code from "lastMapping" to "mapping":
      // First check if there is a new line in between.
      if (lastGeneratedLine < mapping.generatedLine) {
        var code = "";
        // Associate first line with "lastMapping"
        addMappingWithCode(lastMapping, shiftNextLine());
        lastGeneratedLine++;
        lastGeneratedColumn = 0;
        // The remaining code is added without mapping
      } else {
        // There is no new line in between.
        // Associate the code between "lastGeneratedColumn" and
        // "mapping.generatedColumn" with "lastMapping"
        var nextLine = remainingLines[0];
        var code = nextLine.substr(0, mapping.generatedColumn -
                                      lastGeneratedColumn);
        remainingLines[0] = nextLine.substr(mapping.generatedColumn -
                                            lastGeneratedColumn);
        lastGeneratedColumn = mapping.generatedColumn;
        addMappingWithCode(lastMapping, code);
        // No more remaining code, continue
        lastMapping = mapping;
        return;
      }
    }
    // We add the generated code until the first mapping
    // to the SourceNode without any mapping.
    // Each line is added as separate string.
    while (lastGeneratedLine < mapping.generatedLine) {
      node.add(shiftNextLine());
      lastGeneratedLine++;
    }
    if (lastGeneratedColumn < mapping.generatedColumn) {
      var nextLine = remainingLines[0];
      node.add(nextLine.substr(0, mapping.generatedColumn));
      remainingLines[0] = nextLine.substr(mapping.generatedColumn);
      lastGeneratedColumn = mapping.generatedColumn;
    }
    lastMapping = mapping;
  }, this);
  // We have processed all mappings.
  if (remainingLines.length > 0) {
    if (lastMapping) {
      // Associate the remaining code in the current line with "lastMapping"
      addMappingWithCode(lastMapping, shiftNextLine());
    }
    // and add the remaining lines without any mapping
    node.add(remainingLines.join(""));
  }

  // Copy sourcesContent into SourceNode
  aSourceMapConsumer.sources.forEach(function (sourceFile) {
    var content = aSourceMapConsumer.sourceContentFor(sourceFile);
    if (content) {
      node.setSourceContent(sourceFile, content);
    }
  });

  return node;

  function addMappingWithCode(mapping, code) {
    if (mapping === null || mapping.source === undefined) {
      node.add(code);
    } else {
      node.add(new SourceNode(mapping.originalLine,
                              mapping.originalColumn,
                              mapping.source,
                              code,
                              mapping.name));
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.MOZ_SourceMap.SourceNode.prototype"></a>[module uglifyjs.MOZ_SourceMap.SourceNode.prototype](#apidoc.module.uglifyjs.MOZ_SourceMap.SourceNode.prototype)

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.add"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>add (aChunk)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.add)
- description and source-code
```javascript
function SourceNode_add(aChunk) {
  if (Array.isArray(aChunk)) {
    aChunk.forEach(function (chunk) {
      this.add(chunk);
    }, this);
  }
  else if (aChunk instanceof SourceNode || typeof aChunk === "string") {
    if (aChunk) {
      this.children.push(aChunk);
    }
  }
  else {
    throw new TypeError(
      "Expected a SourceNode, string, or an array of SourceNodes and strings. Got " + aChunk
    );
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.join"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>join (aSep)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.join)
- description and source-code
```javascript
function SourceNode_join(aSep) {
  var newChildren;
  var i;
  var len = this.children.length;
  if (len > 0) {
    newChildren = [];
    for (i = 0; i < len-1; i++) {
      newChildren.push(this.children[i]);
      newChildren.push(aSep);
    }
    newChildren.push(this.children[i]);
    this.children = newChildren;
  }
  return this;
}
```
- example usage
```shell
...
arg_parameter_pairs.forEach(function(pair) {
    var splitAt = pair.lastIndexOf(":");

    args.push(pair.substr(0, splitAt));
    parameters.push(pair.substr(splitAt + 1));
});

var wrapped_tl = "(function(" + parameters.join(",") + "){ '$ORIG'; })(" + args.join(",") + ")";
wrapped_tl = parse(wrapped_tl);
wrapped_tl = wrapped_tl.transform(new TreeTransformer(function before(node){
    if (node instanceof AST_Directive && node.value == "$ORIG") {
        return MAP.splice(self.body);
    }
}));
return wrapped_tl;
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.prepend"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>prepend (aChunk)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.prepend)
- description and source-code
```javascript
function SourceNode_prepend(aChunk) {
  if (Array.isArray(aChunk)) {
    for (var i = aChunk.length-1; i >= 0; i--) {
      this.prepend(aChunk[i]);
    }
  }
  else if (aChunk instanceof SourceNode || typeof aChunk === "string") {
    this.children.unshift(aChunk);
  }
  else {
    throw new TypeError(
      "Expected a SourceNode, string, or an array of SourceNodes and strings. Got " + aChunk
    );
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.replaceRight"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>replaceRight (aPattern, aReplacement)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.replaceRight)
- description and source-code
```javascript
function SourceNode_replaceRight(aPattern, aReplacement) {
  var lastChild = this.children[this.children.length - 1];
  if (lastChild instanceof SourceNode) {
    lastChild.replaceRight(aPattern, aReplacement);
  }
  else if (typeof lastChild === 'string') {
    this.children[this.children.length - 1] = lastChild.replace(aPattern, aReplacement);
  }
  else {
    this.children.push(''.replace(aPattern, aReplacement));
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.setSourceContent"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>setSourceContent (aSourceFile, aSourceContent)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.setSourceContent)
- description and source-code
```javascript
function SourceNode_setSourceContent(aSourceFile, aSourceContent) {
  this.sourceContents[util.toSetString(aSourceFile)] = aSourceContent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.toString"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>toString ()](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.toString)
- description and source-code
```javascript
function SourceNode_toString() {
  var str = "";
  this.walk(function (chunk) {
    str += chunk;
  });
  return str;
}
```
- example usage
```shell
...
It enables some transformations that *might* break code logic in certain
contrived cases, but should be fine for most code.  You might want to try it
on your own code, it should reduce the minified size.  Here's what happens
when this flag is on:

- 'new Array(1, 2, 3)' or 'Array(1, 2, 3)' → '[1, 2, 3 ]'
- 'new Object()' → '{}'
- 'String(exp)' or 'exp.toString()' → '"" + exp'
- 'new Object/RegExp/Function/Error/Array (...)' → we discard the 'new'
- 'typeof foo == "undefined"' → 'foo === void 0'
- 'void 0' → 'undefined' (if there is a variable named "undefined" in
  scope; we do it because the variable name will be mangled, typically
  reduced to a single character).

### Conditional compilation
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.toStringWithSourceMap"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>toStringWithSourceMap (aArgs)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.toStringWithSourceMap)
- description and source-code
```javascript
function SourceNode_toStringWithSourceMap(aArgs) {
  var generated = {
    code: "",
    line: 1,
    column: 0
  };
  var map = new SourceMapGenerator(aArgs);
  var sourceMappingActive = false;
  var lastOriginalSource = null;
  var lastOriginalLine = null;
  var lastOriginalColumn = null;
  var lastOriginalName = null;
  this.walk(function (chunk, original) {
    generated.code += chunk;
    if (original.source !== null
        && original.line !== null
        && original.column !== null) {
      if(lastOriginalSource !== original.source
         || lastOriginalLine !== original.line
         || lastOriginalColumn !== original.column
         || lastOriginalName !== original.name) {
        map.addMapping({
          source: original.source,
          original: {
            line: original.line,
            column: original.column
          },
          generated: {
            line: generated.line,
            column: generated.column
          },
          name: original.name
        });
      }
      lastOriginalSource = original.source;
      lastOriginalLine = original.line;
      lastOriginalColumn = original.column;
      lastOriginalName = original.name;
      sourceMappingActive = true;
    } else if (sourceMappingActive) {
      map.addMapping({
        generated: {
          line: generated.line,
          column: generated.column
        }
      });
      lastOriginalSource = null;
      sourceMappingActive = false;
    }
    chunk.match(REGEX_CHARACTER).forEach(function (ch, idx, array) {
      if (REGEX_NEWLINE.test(ch)) {
        generated.line++;
        generated.column = 0;
        // Mappings end at eol
        if (idx + 1 === array.length) {
          lastOriginalSource = null;
          sourceMappingActive = false;
        } else if (sourceMappingActive) {
          map.addMapping({
            source: original.source,
            original: {
              line: original.line,
              column: original.column
            },
            generated: {
              line: generated.line,
              column: generated.column
            },
            name: original.name
          });
        }
      } else {
        generated.column += ch.length;
      }
    });
  });
  this.walkSourceContents(function (sourceFile, sourceContent) {
    map.setSourceContent(sourceFile, sourceContent);
  });

  return { code: generated.code, map: map };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.walk"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>walk (aFn)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.walk)
- description and source-code
```javascript
function SourceNode_walk(aFn) {
  var chunk;
  for (var i = 0, len = this.children.length; i < len; i++) {
    chunk = this.children[i];
    if (chunk instanceof SourceNode) {
      chunk.walk(aFn);
    }
    else {
      if (chunk !== '') {
        aFn(chunk, { source: this.source,
                     line: this.line,
                     column: this.column,
                     name: this.name });
      }
    }
  }
}
```
- example usage
```shell
...
    return wrapped_tl;
},
wrap_commonjs: function(name, export_all) {
    var self = this;
    var to_export = [];
    if (export_all) {
        self.figure_out_scope();
        self.walk(new TreeWalker(function(node){
            if (node instanceof AST_SymbolDeclaration && node.definition().global) {
                if (!find_if(function(n){ return n.name == node.name }, to_export))
                    to_export.push(node);
            }
        }));
    }
    var wrapped_tl = "(function(exports, global){ global['" + name + "'] = exports; '$ORIG'; '$EXPORTS'; }({}, (function(){return
 this}())))";
...
```

#### <a name="apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.walkSourceContents"></a>[function <span class="apidocSignatureSpan">uglifyjs.MOZ_SourceMap.SourceNode.prototype.</span>walkSourceContents (aFn)](#apidoc.element.uglifyjs.MOZ_SourceMap.SourceNode.prototype.walkSourceContents)
- description and source-code
```javascript
function SourceNode_walkSourceContents(aFn) {
  for (var i = 0, len = this.children.length; i < len; i++) {
    if (this.children[i] instanceof SourceNode) {
      this.children[i].walkSourceContents(aFn);
    }
  }

  var sources = Object.keys(this.sourceContents);
  for (var i = 0, len = sources.length; i < len; i++) {
    aFn(util.fromSetString(sources[i]), this.sourceContents[sources[i]]);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.SymbolDef"></a>[module uglifyjs.SymbolDef](#apidoc.module.uglifyjs.SymbolDef)

#### <a name="apidoc.element.uglifyjs.SymbolDef.SymbolDef"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>SymbolDef (scope, index, orig)](#apidoc.element.uglifyjs.SymbolDef.SymbolDef)
- description and source-code
```javascript
function SymbolDef(scope, index, orig) {
    this.name = orig.name;
    this.orig = [ orig ];
    this.scope = scope;
    this.references = [];
    this.global = false;
    this.mangled_name = null;
    this.undeclared = false;
    this.constant = false;
    this.index = index;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.SymbolDef.prototype"></a>[module uglifyjs.SymbolDef.prototype](#apidoc.module.uglifyjs.SymbolDef.prototype)

#### <a name="apidoc.element.uglifyjs.SymbolDef.prototype.mangle"></a>[function <span class="apidocSignatureSpan">uglifyjs.SymbolDef.prototype.</span>mangle (options)](#apidoc.element.uglifyjs.SymbolDef.prototype.mangle)
- description and source-code
```javascript
mangle = function (options) {
    if (!this.mangled_name && !this.unmangleable(options)) {
        var s = this.scope;
        if (!options.screw_ie8 && this.orig[0] instanceof AST_SymbolLambda)
            s = s.parent_scope;
        this.mangled_name = s.next_mangled(options, this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.SymbolDef.prototype.unmangleable"></a>[function <span class="apidocSignatureSpan">uglifyjs.SymbolDef.prototype.</span>unmangleable (options)](#apidoc.element.uglifyjs.SymbolDef.prototype.unmangleable)
- description and source-code
```javascript
unmangleable = function (options) {
    if (!options) options = {};

    return (this.global && !options.toplevel)
        || this.undeclared
        || (!options.eval && (this.scope.uses_eval || this.scope.uses_with))
        || (options.keep_fnames
            && (this.orig[0] instanceof AST_SymbolLambda
                || this.orig[0] instanceof AST_SymbolDefun));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.TreeWalker"></a>[module uglifyjs.TreeWalker](#apidoc.module.uglifyjs.TreeWalker)

#### <a name="apidoc.element.uglifyjs.TreeWalker.TreeWalker"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>TreeWalker (callback)](#apidoc.element.uglifyjs.TreeWalker.TreeWalker)
- description and source-code
```javascript
function TreeWalker(callback) {
    this.visit = callback;
    this.stack = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.TreeWalker.prototype"></a>[module uglifyjs.TreeWalker.prototype](#apidoc.module.uglifyjs.TreeWalker.prototype)

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype._visit"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>_visit (node, descend)](#apidoc.element.uglifyjs.TreeWalker.prototype._visit)
- description and source-code
```javascript
_visit = function (node, descend) {
    this.stack.push(node);
    var ret = this.visit(node, descend ? function(){
        descend.call(node);
    } : noop);
    if (!ret && descend) {
        descend.call(node);
    }
    this.stack.pop();
    return ret;
}
```
- example usage
```shell
...
    },
    $documentation: "Base class of all AST nodes",
    $propdoc: {
        start: "[AST_Token] The first token of this node",
        end: "[AST_Token] The last token of this node"
    },
    _walk: function(visitor) {
        return visitor._visit(this);
    },
    walk: function(visitor) {
        return this._walk(visitor); // not sure the indirection will be any help
    }
}, null);

AST_Node.warn_function = null;
...
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.find_parent"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>find_parent (type)](#apidoc.element.uglifyjs.TreeWalker.prototype.find_parent)
- description and source-code
```javascript
find_parent = function (type) {
    var stack = this.stack;
    for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof type) return x;
    }
}
```
- example usage
```shell
...
    var stack = this.stack;
    for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof type) return x;
    }
},
has_directive: function(type) {
    return this.find_parent(AST_Scope).has_directive(type);
},
in_boolean_context: function() {
    var stack = this.stack;
    var i = stack.length, self = stack[--i];
    while (i > 0) {
        var p = stack[--i];
        if ((p instanceof AST_If           && p.condition === self) ||
...
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.has_directive"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>has_directive (type)](#apidoc.element.uglifyjs.TreeWalker.prototype.has_directive)
- description and source-code
```javascript
has_directive = function (type) {
    return this.find_parent(AST_Scope).has_directive(type);
}
```
- example usage
```shell
...
    var stack = this.stack;
    for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof type) return x;
    }
},
has_directive: function(type) {
    return this.find_parent(AST_Scope).has_directive(type);
},
in_boolean_context: function() {
    var stack = this.stack;
    var i = stack.length, self = stack[--i];
    while (i > 0) {
        var p = stack[--i];
        if ((p instanceof AST_If           && p.condition === self) ||
...
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.in_boolean_context"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>in_boolean_context ()](#apidoc.element.uglifyjs.TreeWalker.prototype.in_boolean_context)
- description and source-code
```javascript
in_boolean_context = function () {
    var stack = this.stack;
    var i = stack.length, self = stack[--i];
    while (i > 0) {
        var p = stack[--i];
        if ((p instanceof AST_If           && p.condition === self) ||
            (p instanceof AST_Conditional  && p.condition === self) ||
            (p instanceof AST_DWLoop       && p.condition === self) ||
            (p instanceof AST_For          && p.condition === self) ||
            (p instanceof AST_UnaryPrefix  && p.operator == "!" && p.expression === self))
        {
            return true;
        }
        if (!(p instanceof AST_Binary && (p.operator == "&&" || p.operator == "||")))
            return false;
        self = p;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.loopcontrol_target"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>loopcontrol_target (label)](#apidoc.element.uglifyjs.TreeWalker.prototype.loopcontrol_target)
- description and source-code
```javascript
loopcontrol_target = function (label) {
    var stack = this.stack;
    if (label) for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof AST_LabeledStatement && x.label.name == label.name) {
            return x.body;
        }
    } else for (var i = stack.length; --i >= 0;) {
        var x = stack[i];
        if (x instanceof AST_Switch || x instanceof AST_IterationStatement)
            return x;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.parent"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>parent (n)](#apidoc.element.uglifyjs.TreeWalker.prototype.parent)
- description and source-code
```javascript
parent = function (n) {
    return this.stack[this.stack.length - 2 - (n || 0)];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.pop"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>pop ()](#apidoc.element.uglifyjs.TreeWalker.prototype.pop)
- description and source-code
```javascript
pop = function () {
    return this.stack.pop();
}
```
- example usage
```shell
...
    this.stack.push(node);
    var ret = this.visit(node, descend ? function(){
        descend.call(node);
    } : noop);
    if (!ret && descend) {
        descend.call(node);
    }
    this.stack.pop();
    return ret;
},
parent: function(n) {
    return this.stack[this.stack.length - 2 - (n || 0)];
},
push: function (node) {
    this.stack.push(node);
...
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.push"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>push (node)](#apidoc.element.uglifyjs.TreeWalker.prototype.push)
- description and source-code
```javascript
push = function (node) {
    this.stack.push(node);
}
```
- example usage
```shell
...
    code += "this.initialize();";
code += "}}";
var ctor = new Function(code)();
if (proto) {
    ctor.prototype = proto;
    ctor.BASE = base;
}
if (base) base.SUBCLASSES.push(ctor);
ctor.prototype.CTOR = ctor;
ctor.PROPS = props || null;
ctor.SELF_PROPS = self_props;
ctor.SUBCLASSES = [];
if (type) {
    ctor.prototype.TYPE = ctor.TYPE = type;
}
...
```

#### <a name="apidoc.element.uglifyjs.TreeWalker.prototype.self"></a>[function <span class="apidocSignatureSpan">uglifyjs.TreeWalker.prototype.</span>self ()](#apidoc.element.uglifyjs.TreeWalker.prototype.self)
- description and source-code
```javascript
self = function () {
    return this.stack[this.stack.length - 1];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.uglifyjs.base54"></a>[module uglifyjs.base54](#apidoc.module.uglifyjs.base54)

#### <a name="apidoc.element.uglifyjs.base54.base54"></a>[function <span class="apidocSignatureSpan">uglifyjs.</span>base54 (num)](#apidoc.element.uglifyjs.base54.base54)
- description and source-code
```javascript
function base54(num) {
    var ret = "", base = 54;
    num++;
    do {
        num--;
        ret += String.fromCharCode(chars[num % base]);
        num = Math.floor(num / base);
        base = 64;
    } while (num > 0);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.base54.consider"></a>[function <span class="apidocSignatureSpan">uglifyjs.base54.</span>consider (str)](#apidoc.element.uglifyjs.base54.consider)
- description and source-code
```javascript
consider = function (str){
    for (var i = str.length; --i >= 0;) {
        var code = str.charCodeAt(i);
        if (code in frequency) ++frequency[code];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.base54.freq"></a>[function <span class="apidocSignatureSpan">uglifyjs.base54.</span>freq ()](#apidoc.element.uglifyjs.base54.freq)
- description and source-code
```javascript
freq = function (){ return frequency }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.base54.get"></a>[function <span class="apidocSignatureSpan">uglifyjs.base54.</span>get ()](#apidoc.element.uglifyjs.base54.get)
- description and source-code
```javascript
get = function (){ return chars }
```
- example usage
```shell
...
set: function(key, val) {
    if (!this.has(key)) ++this._size;
    this._values["$" + key] = val;
    return this;
},
add: function(key, val) {
    if (this.has(key)) {
        this.get(key).push(val);
    } else {
        this.set(key, [ val ]);
    }
    return this;
},
get: function(key) { return this._values["$" + key] },
del: function(key) {
...
```

#### <a name="apidoc.element.uglifyjs.base54.reset"></a>[function <span class="apidocSignatureSpan">uglifyjs.base54.</span>reset ()](#apidoc.element.uglifyjs.base54.reset)
- description and source-code
```javascript
function reset() {
    frequency = Object.create(null);
    chars = string.split("").map(function(ch){ return ch.charCodeAt(0) });
    chars.forEach(function(ch){ frequency[ch] = 0 });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.uglifyjs.base54.sort"></a>[function <span class="apidocSignatureSpan">uglifyjs.base54.</span>sort ()](#apidoc.element.uglifyjs.base54.sort)
- description and source-code
```javascript
sort = function () {
    chars = mergeSort(chars, function(a, b){
        if (is_digit(a) && !is_digit(b)) return 1;
        if (is_digit(b) && !is_digit(a)) return -1;
        return frequency[b] - frequency[a];
    });
}
```
- example usage
```shell
...
    f += "switch(str){";
    for (var i = 0; i < arr.length; ++i) f += "case " + JSON.stringify(arr[i]) + ":";
    f += "return true}return false;";
}
// When there are more than three length categories, an outer
// switch first dispatches on the lengths, to save on comparisons.
if (cats.length > 3) {
    cats.sort(function(a, b) {return b.length - a.length;});
    f += "switch(str.length){";
    for (var i = 0; i < cats.length; ++i) {
        var cat = cats[i];
        f += "case " + cat[0].length + ":";
        compareTo(cat);
    }
    f += "}";
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
