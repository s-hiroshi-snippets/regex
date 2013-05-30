PhpStorm
-----

### コメント処理1

    <!-- ?/([a-z0-9-_]+) ?-->

    <!-- $1 -->


before

    <!-- /id_or-scelector -->

after

    <!-- id_or_selector -->


### コメント処理2

    ^( +)(<!-- /?[a-zA-Z0-9-_]+ -->)(.+)$


    $1$3$2

before

    <!-- content --></div>

after

    </div><!-- content -->

### フォーマット

    \(([^ )]+)

    ( $1