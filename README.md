SpringDataRedisCacheSample
==========================

Spring data redis cache sample

This is an cached method
  @Cacheable(value="cache1", condition="#test.equals(#test)")
    public String sayHello(String test) {
        DateFormat dateFormat = new SimpleDateFormat("yyyy/MM/dd HH:mm:ss");
        Date date = new Date();
        return "test! "+dateFormat.format(date);
    }
    
package foo.bar.config; -> RedisConfig you can configure the redis cache manager bean
i hold the cachedBeans value on Map resources its more configurable than hardcoding
    

    