# GroundHogDay.cs
Web-API for [groundhog-day.com](https://groundhog-day.com) an leading data source for North America’s prognosticating groundhogs and their yearly predictions

## Example
```cs
using System;
using GroundHogDayApi;
using System.Threading.Tasks;

namespace Application
{
    internal class Program
    {
        static async Task Main()
        {
            var api = new GroundHogDay();
            string groundHogs = await api.getGroundHogs();
            Console.WriteLine(groundHogs);
        }
    }
}
```
