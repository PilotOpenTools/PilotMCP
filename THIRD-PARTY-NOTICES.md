# Сторонние компоненты

Исходный код PilotMCP распространяется по лицензии [Apache 2.0](LICENSE). Релизные архивы (`PilotMCP-v<версия>-win-x64.zip`, `PilotMCP-v<версия>-win-x64-selfcontained.zip` и `.mcpb`) содержат сторонние библиотеки на их собственных условиях. Список ниже составлен по метаданным пакетов NuGet (лицензия и сайт берутся из `.nuspec`) для файлов, которые попадают в архив `win-x64`. Тексты лицензий лежат в папке [`licenses`](licenses).

## MuPDFCore: AGPL-3.0

Пакеты `MuPDFCore` и `MuPDFCore.NativeAssets.*` (версия 2.0.1, автор Giorgio Bianchini) распространяются по лицензии [AGPL-3.0-only](licenses/AGPL-3.0.txt) и включают нативную библиотеку MuPDF. PilotMCP использует их только для отрисовки страниц XPS в PNG (`Tools/DocumentTools.cs`, `GetDocumentPageImage`); для PDF используется PDFium (PDFtoImage), текст извлекает PdfPig.

Эти библиотеки входят в релизные архивы. При распространении сборок, содержащих MuPDFCore, действуют условия AGPL-3.0, в том числе раздел 6 (передача исходного кода). Исходный код:

- PilotMCP: [github.com/PilotOpenTools/PilotMCP](https://github.com/PilotOpenTools/PilotMCP), нужный тег релиза;
- MuPDFCore 2.0.1: [github.com/arklumpus/MuPDFCore](https://github.com/arklumpus/MuPDFCore).

## Остальные компоненты

- Пакеты под MIT: условия в [licenses/MIT.txt](licenses/MIT.txt), правообладатели указаны на сайтах пакетов (см. таблицу ниже).
- Пакеты под Apache-2.0: текст лицензии совпадает с [LICENSE](LICENSE).
- `UglyToad.PdfPig` 1.7.0-custom-5 (пользовательская сборка PdfPig, у оригинального проекта лицензия Apache-2.0): в метаданных пакета лицензия не указана.
- Среда выполнения .NET в самосодержащем архиве: MIT, [dotnet/runtime](https://github.com/dotnet/runtime/blob/main/LICENSE.TXT).

## Пакеты NuGet в архиве win-x64

Всего 74.

| Пакет | Версия | Лицензия | Сайт |
| --- | --- | --- | --- |
| Ascon.Pilot.Server.Api | 26.21.0 | Apache-2.0 | http://pilotems.com/ |
| bblanchon.PDFium.Win32 | 139.0.7215 | Apache-2.0 | https://github.com/bblanchon/pdfium-binaries |
| log4net | 3.3.0 | Apache-2.0 | https://logging.apache.org/log4net/ |
| Microsoft.AspNetCore.Cryptography.Internal | 9.0.21 | MIT | https://asp.net/ |
| Microsoft.AspNetCore.DataProtection | 9.0.21 | MIT | https://asp.net/ |
| Microsoft.AspNetCore.DataProtection.Abstractions | 9.0.21 | MIT | https://asp.net/ |
| Microsoft.AspNetCore.DataProtection.Extensions | 9.0.21 | MIT | https://asp.net/ |
| Microsoft.Bcl.Cryptography | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.AI.Abstractions | 9.5.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.Abstractions | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.Binder | 8.0.2 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.CommandLine | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.EnvironmentVariables | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.FileExtensions | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.Json | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Configuration.UserSecrets | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.DependencyInjection | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.DependencyInjection.Abstractions | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.Diagnostics | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Diagnostics.Abstractions | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.FileProviders.Abstractions | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.FileProviders.Physical | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.FileSystemGlobbing | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.Hosting | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Hosting.Abstractions | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging.Abstractions | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging.Configuration | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging.Console | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging.Debug | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging.EventLog | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.Logging.EventSource | 8.0.1 | MIT | https://dot.net/ |
| Microsoft.Extensions.ObjectPool | 8.0.10 | MIT | https://asp.net/ |
| Microsoft.Extensions.Options | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Extensions.Options.ConfigurationExtensions | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.Primitives | 9.0.21 | MIT | https://dot.net/ |
| Microsoft.Win32.Registry | 5.0.0 | MIT | https://github.com/dotnet/runtime |
| ModelContextProtocol | 0.2.0-preview.1 | MIT | https://github.com/modelcontextprotocol/csharp-sdk |
| MuPDFCore | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Linux-arm64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Linux-musl-arm64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Linux-musl-x64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Linux-x64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Mac-arm64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Mac-x64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Win-arm64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Win-x64 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| MuPDFCore.NativeAssets.Win-x86 | 2.0.1 | AGPL-3.0-only | https://github.com/arklumpus/MuPDFCore |
| Newtonsoft.Json | 13.0.4 | MIT | https://www.newtonsoft.com/json |
| PDFtoImage | 5.2.0 | MIT | https://github.com/sungaila/PDFtoImage |
| protobuf-net | 3.2.56 | Apache-2.0 | https://github.com/protobuf-net/protobuf-net |
| protobuf-net.Core | 3.2.56 | Apache-2.0 | https://github.com/protobuf-net/protobuf-net |
| SkiaSharp | 3.119.2 | MIT | https://go.microsoft.com/fwlink/?linkid=868515 |
| SkiaSharp.NativeAssets.Win32 | 3.119.2 | MIT | https://go.microsoft.com/fwlink/?linkid=868515 |
| System.Configuration.ConfigurationManager | 8.0.1 | MIT | https://dot.net/ |
| System.Diagnostics.DiagnosticSource | 9.0.21 | MIT | https://dot.net/ |
| System.Diagnostics.EventLog | 8.0.1 | MIT | https://dot.net/ |
| System.Formats.Asn1 | 9.0.21 | MIT | https://dot.net/ |
| System.IO.Pipelines | 8.0.0 | MIT | https://dot.net/ |
| System.Net.ServerSentEvents | 10.0.0-preview.3.25171.5 | MIT | https://dot.net/ |
| System.Security.AccessControl | 5.0.0 | MIT | https://github.com/dotnet/runtime |
| System.Security.Cryptography.Pkcs | 9.0.21 | MIT | https://dot.net/ |
| System.Security.Cryptography.ProtectedData | 8.0.0 | MIT | https://dot.net/ |
| System.Security.Cryptography.Xml | 9.0.21 | MIT | https://dot.net/ |
| System.Security.Permissions | 8.0.0 | MIT | https://dot.net/ |
| System.Security.Principal.Windows | 5.0.0 | MIT | https://github.com/dotnet/runtime |
| System.ServiceModel.Primitives | 8.1.2 | MIT | https://github.com/dotnet/wcf |
| System.Windows.Extensions | 8.0.0 | MIT | https://dot.net/ |
| UglyToad.PdfPig | 1.7.0-custom-5 | не указана в метаданных пакета | — |
| UglyToad.PdfPig.Core | 1.7.0-custom-5 | не указана в метаданных пакета | — |
| UglyToad.PdfPig.Fonts | 1.7.0-custom-5 | не указана в метаданных пакета | — |
| UglyToad.PdfPig.Tokenization | 1.7.0-custom-5 | не указана в метаданных пакета | — |
| UglyToad.PdfPig.Tokens | 1.7.0-custom-5 | не указана в метаданных пакета | — |
