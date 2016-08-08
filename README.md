Vietnamese (without diacritics - Tiếng Việt không dấu) Analysis Plugin for Elasticsearch
========================================

Vietnamese (without diacritics) Analysis plugin integrates Vietnamese language without diacritics analysis into Elasticsearch.

In order to install the plugin, simply run:

```sh
bin/plugin install https://raw.githubusercontent.com/tam-vo/elasticsearch-analysis-vietnamese-without-diacritics/master/install/elasticsearch-analysis-vietnamese-0.2.3.zip

```

Or to build from source, you need to build it with Maven:

```bash
mvn clean package
bin/plugin install file:target/releases/elasticsearch-analysis-vietnamese-0.2.3.zip
```

*Notes*: To build the plugin you need to clone and build the [vn-nlp-libararies](https://github.com/yldbk/vn-nlp-libraries). The plugin uses  [Lê Hồng Phương](http://mim.hus.vnu.edu.vn/phuonglh/) vnTokenizer library customizable version for Vietnamese without diacritics. Thanks thầy Lê Hồng Phương for great contribution.

|Vietnamese Analysis Plugin|Elasticsearch|
|---|---|
| master|2.3.2|
| 0.2.2|2.2.0|
| 0.2.1.1|2.1.1|
| 0.2.1|2.1.0|
| 0.2|2.0.0|
| 0.1.7|1.7+|
| 0.1.6|1.6+|
| 0.1.5|1.5+|
| 0.1.1|1.4+|
| 0.1|1.3|


## User guide

The plugin includes the `vi_analyzer` analyzer and `vi_tokenizer` tokenizer.

The `vi_analyzer` is built using the `vi_tokenizer` tokenizer.

 The analyzer analyzes `"Cong nghe thong tin Viet Nam"` `(without diacritics - Tiếng Việt Không dấu)` into `"Cong nghe thong tin"` and `"Viet Nam"` tokens.

License
-------

    This software is licensed under the Apache 2 license, quoted below.

    Licensed under the Apache License, Version 2.0 (the "License"); you may not
    use this file except in compliance with the License. You may obtain a copy of
    the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
    License for the specific language governing permissions and limitations under
    the License.
