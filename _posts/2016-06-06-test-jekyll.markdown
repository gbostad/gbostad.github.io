---
layout: post
title:  "Test jekyll and stuff"
---

Test highlighting, some code from Postgresql documentation

{% highlight sql linenos %}
WITH RECURSIVE t(n) AS (
    VALUES (1)
  UNION ALL
    SELECT n+1 FROM t WHERE n < 100
)
SELECT sum(n) FROM t;
{% endhighlight %}


Test highlighting, some code from Postgresql documentation

{% highlight plpgsql linenos %}
CREATE FUNCTION logfunc2(logtxt text) RETURNS void AS $$
    DECLARE
        curtime timestamp;
    BEGIN
        curtime := 'now';
        INSERT INTO logtable VALUES (logtxt, curtime);
    END;
$$ LANGUAGE plpgsql;
{% endhighlight %}
