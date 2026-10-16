FROM mcr.microsoft.com/dotnet/aspnet:10.0

RUN apt-get update && apt-get install -y libgdiplus

WORKDIR /app

EXPOSE 80

COPY ./ /app

ENV TZ=Asia/Shanghai
ENV ASPNETCORE_HTTP_PORTS=80

ENTRYPOINT ["dotnet", "CoreCms.Net.Web.Admin.dll"]