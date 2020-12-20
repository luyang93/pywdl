# pywdl

## Checklist

- Top priority denoted as "**(!!)**".

### WDL -> Python string Transforms

Compilation design; expression are stored as Python code as strings in collections.

- Types
  * [X] Primitives (String, Int, Float, Boolean, File)
    - [ ] Directory
  * [X] Compound (Array, Pair, Map)
  * [ ] Struct
- Expression
  * [X] LOR, LAND
  * [ ] ==, !==, <=, >=, <, > **(!!)**
  * [ ] +, - **(!!)**
  * [ ] *, /, % **(!!)**
  * [ ] <=, <, =, >, >= **(!!)**
  * [X] apply (function call)
    - [ ] allow user to hook into this to modify how arguments are parsed. **(!!)**
  * [X] array_literal
  * [X] pair_literal
  * [ ] map_literal
  * [ ] struct_literal
  * [X] ifthenelse
  * [X] expression_group
  * [ ] get_name **(!!)**
  * [ ] negate **(!!)**
  * [ ] unirarysigned
  * [ ] primitives __should work? needs testing__
  * [ ] left_name
- Document
  * [ ] import
  * [ ] meta
- Workflow
  * [X] input
  * [X] call
  * [X] scatter
  * [X] conditional
  * [X] output
- Task
  * [ ] input **(!!)**
  * [ ] runtime **(!!)**
  * [ ] command **(!!)**
  * [ ] output **(!!)**

### Antlr4 to objects Transforms


## Credits

The following files come from [openwdl](https://github.com/openwdl/wdl/tree/main/versions/development/parsers/antlr4) with license: https://github.com/openwdl/wdl/blob/main/LICENSE. 

- [WdlLexer.g4](pywdl/antlr/WdlLexer.g4)
- [WdlParser.g4](pywdl/antlr/WdlParser.g4)

The following file is modified from [Toil](https://github.com/DataBiosphere/toil/) with license: https://github.com/DataBiosphere/toil/blob/master/LICENSE

- [wdl_parser.py](https://github.com/DataBiosphere/toil/blob/master/src/toil/wdl/wdl_types.py)
